<template>
  <div>
    <header class="bg-white">
      <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
        <div class="flex lg:flex-1">
          <nuxt-link to="/checklist" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="" />
          </nuxt-link>
        </div>
        <div class="flex flex-1 justify-end">
          <nuxt-link to="/" class="text-sm font-semibold leading-6 text-gray-900">Log out <span
              aria-hidden="true">&rarr;</span></nuxt-link>
        </div>
      </nav>
    </header>
    <main class="bg-white">
      <div class="mx-auto max-w-7xl p-6 lg:px-8">
        <div class="flex justify-between">
          <h2 class="text-2xl font-bold tracking-tight text-gray-900">
            Checklist
          </h2>
          <button type="button"
            class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
            Create
          </button>
        </div>
        <div class="mt-6 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-4 xl:gap-x-8">

          <ChecklistCard />

        </div>
      </div>
    </main>
  </div>
</template>

<script>
import ChecklistCard from "@/components/checklistcmp/checklistCard.vue";

export default {
  components: {
    ChecklistCard,
  }
}
</script>