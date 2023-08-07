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
            Checklist title
          </h2>
          <div>
            <button type="button"
              class="rounded-md bg-gray-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-gray-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-gray-600">
              Reload
            </button>
            <button type="button"
              class="rounded-md bg-green-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-green-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-green-600">
              Excel upload
            </button>
            <button type="button"
              class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
              Add item
            </button>
            <button type="button"
              class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
              Save
            </button>
          </div>
        </div>
        <div class="mt-4 -mb-3">
          <div class="not-prose relative bg-slate-50 rounded-xl overflow-hidden dark:bg-slate-800/25">
            <div style="background-position: 10px 10px"
              class="absolute inset-0 bg-grid-slate-100 [mask-image:linear-gradient(0deg,#fff,rgba(255,255,255,0.6))] dark:bg-grid-slate-700/25 dark:[mask-image:linear-gradient(0deg,rgba(255,255,255,0.1),rgba(255,255,255,0.5))]">
            </div>
            <div class="relative rounded-xl overflow-auto">
              <div class="shadow-sm overflow-hidden my-8">
                <table class="border-collapse table-auto w-full text-sm">
                  <thead>
                    <tr>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Category
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Product name
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Brand
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Need status
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Purchase status
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        Notes
                      </th>
                      <th class="border-b font-medium p-4 pt-0 pb-3 text-slate-400 text-center">
                        buttons
                      </th>
                    </tr>
                  </thead>

                  <tbody class="bg-white">
                    <tr>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        Category1
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        Malcolm Lockyer
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        1961
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        1961
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        1961
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        1961
                      </td>
                      <td class="border-b border-slate-100 p-4 text-slate-500 text-center">
                        <button class="text-sm font-medium text-red-500">
                          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                              d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                          </svg>
                        </button>
                      </td>
                    </tr>
                  </tbody>

                </table>
              </div>
            </div>
            <div class="absolute inset-0 pointer-events-none border border-black/5 rounded-xl dark:border-white/5"></div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {

}
</script>