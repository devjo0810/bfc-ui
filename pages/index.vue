<template>
  <div class="flex min-h-full flex-col justify-center px-6 py-12 lg:px-8">
    <div class="sm:mx-auto sm:w-full sm:max-w-sm">
      <img class="mx-auto h-10 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
        alt="Your Company" />
      <h2 class="mt-10 text-center text-2xl font-bold leading-9 tracking-tight text-gray-900">
        Sign in to your account
      </h2>
    </div>

    <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
      <form class="space-y-6" @submit.prevent>
        <div>
          <label for="email" class="block text-sm font-medium leading-6 text-gray-900">Email address</label>

          <inputEmail v-model="email" autocomplete="email" />

        </div>

        <div>
          <div class="flex items-center justify-between">
            <label for="password" class="block text-sm font-medium leading-6 text-gray-900">Password</label>
            <div class="text-sm">
              <nuxt-link to="/find" class="font-semibold text-indigo-600 hover:text-indigo-500">
                Forgot password?</nuxt-link>
            </div>
          </div>
          <inputPassword v-model="password" />
        </div>
        <div>
          <nuxt-link to="/login"
            class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
            @click="login">
            Sign in
          </nuxt-link>
          <nuxt-link to="/join"
            class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 mt-2">
            Join
          </nuxt-link>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    email: 'test1@test.com',
    password: 'test1234',
  }),
  methods: {
    async login() {
      const email = this.email
      const password = this.password
      console.log('email: ', email)
      console.log('password: ', password)
      const response = await this.$http.$post(
        'http://146.56.143.153:7075/auth/login',
        {
          email,
          password,
        }
      )
      console.log(response)
    },
  },
}
</script>
