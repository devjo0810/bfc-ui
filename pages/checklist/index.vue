<template>
  <div>
    <header class="bg-white">
      <nav
        class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8"
        aria-label="Global"
      >
        <div class="flex lg:flex-1">
          <nuxt-link to="/checklist" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img
              class="h-8 w-auto"
              src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
              alt=""
            />
          </nuxt-link>
        </div>
        <div class="flex flex-1 justify-end">
          <nuxt-link
            to="/"
            class="text-sm font-semibold leading-6 text-gray-900"
            >Log out <span aria-hidden="true">&rarr;</span></nuxt-link
          >
        </div>
      </nav>
    </header>
    <main class="bg-white">
      <div class="mx-auto max-w-7xl p-6 lg:px-8">
        <div class="flex justify-between">
          <h2 class="text-2xl font-bold tracking-tight text-gray-900">
            Checklist
          </h2>
          <button
            type="button"
            class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
          >
            Create
          </button>
        </div>
        <div
          class="mt-6 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-4 xl:gap-x-8"
        >
          <div class="group relative">
            <nuxt-link
              to="/checklist/detail"
              class="mt-2 flex justify-between border border-gray-300 rounded-md p-3 hover:cursor-pointer"
            >
              <div>
                <h3 class="text-lg text-gray-700">Checklist name</h3>
                <p class="mt-1 text-sm text-gray-500">
                  checklist item count : 26
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  created at : 2023.07.01
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  modified at : 2023.07.02
                </p>
              </div>
              <button class="text-sm font-medium text-red-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                  />
                </svg>
              </button>
            </nuxt-link>
          </div>
          <div class="group relative">
            <nuxt-link
              to="/checklist/detail"
              class="mt-2 flex justify-between border border-gray-300 rounded-md p-3 hover:cursor-pointer"
            >
              <div>
                <h3 class="text-lg text-gray-700">Checklist name</h3>
                <p class="mt-1 text-sm text-gray-500">
                  checklist item count : 26
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  created at : 2023.07.01
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  modified at : 2023.07.02
                </p>
              </div>
              <button class="text-sm font-medium text-red-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                  />
                </svg>
              </button>
            </nuxt-link>
          </div>

          <div class="group relative">
            <nuxt-link
              to="/checklist/detail"
              class="mt-2 flex justify-between border border-gray-300 rounded-md p-3 hover:cursor-pointer"
            >
              <div>
                <h3 class="text-lg text-gray-700">Checklist name</h3>
                <p class="mt-1 text-sm text-gray-500">
                  checklist item count : 26
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  created at : 2023.07.01
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  modified at : 2023.07.02
                </p>
              </div>
              <button class="text-sm font-medium text-red-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                  />
                </svg>
              </button>
            </nuxt-link>
          </div>
          <div class="group relative">
            <nuxt-link
              to="/checklist/detail"
              class="mt-2 flex justify-between border border-gray-300 rounded-md p-3 hover:cursor-pointer"
            >
              <div>
                <h3 class="text-lg text-gray-700">Checklist name</h3>
                <p class="mt-1 text-sm text-gray-500">
                  checklist item count : 26
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  created at : 2023.07.01
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  modified at : 2023.07.02
                </p>
              </div>
              <button class="text-sm font-medium text-red-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                  />
                </svg>
              </button>
            </nuxt-link>
          </div>
          <div class="group relative">
            <nuxt-link
              to="/checklist/detail"
              class="mt-2 flex justify-between border border-gray-300 rounded-md p-3 hover:cursor-pointer"
            >
              <div>
                <h3 class="text-lg text-gray-700">Checklist name</h3>
                <p class="mt-1 text-sm text-gray-500">
                  checklist item count : 26
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  created at : 2023.07.01
                </p>
                <p class="mt-1 text-sm text-gray-500">
                  modified at : 2023.07.02
                </p>
              </div>
              <button class="text-sm font-medium text-red-500">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                  />
                </svg>
              </button>
            </nuxt-link>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>