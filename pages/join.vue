<template>
  <div class="flex min-h-full flex-col justify-center px-6 py-12 lg:px-8">
    <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
      <form @submit.prevent>
        <div class="space-y-12">
          <div class="border-b border-gray-900/10 pb-12">
            <h2 class="text-base font-semibold leading-7 text-gray-900">
              Personal Information
            </h2>
            <p class="mt-1 text-sm leading-6 text-gray-600">
              Use a permanent address where you can receive mail.
            </p>

            <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
              <div class="sm:col-span-6">
                <label for="email" class="block text-sm font-medium leading-6 text-gray-900">Email address</label>
                <div class="mt-2 grid gap-x-6 sm:grid-cols-6">
                  <div class="sm:col-span-4">
                    <inputEmail v-model="email" @input="userEmailInput" autocomplete="email" />
                  </div>
                  <div class="sm:col-span-2">
                    <button
                      class="block w-full rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
                      @click="emailCheck">
                      check
                    </button>
                  </div>
                </div>
              </div>

              <div class="sm:col-span-4">
                <label for="username" class="block text-sm font-medium leading-6 text-gray-900">Username</label>

                <inputEmail v-model="userName" type="text" />

              </div>

              <div class="sm:col-span-4">
                <label for="password" class="block text-sm font-medium leading-6 text-gray-900">Password</label>

                <inputPassword v-model="password" />

              </div>
              <div class="sm:col-span-4">
                <label for="passwordCheck" class="block text-sm font-medium leading-6 text-gray-900">
                  Password Check</label>

                <inputPassword v-model="passwordCheck" @input="passwrodComfirmed" />

              </div>
            </div>
          </div>
        </div>

        <div class="mt-6 flex items-center justify-end gap-x-6">
          <nuxt-link to="/" class="text-sm font-semibold leading-6 text-gray-900">Cancel</nuxt-link>
          <button type="submit"
            class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
            @click="signUp">
            Save
          </button>
        </div>
      </form>
    </div>

    <!--유효성 검사에 따른 팝업알림-->
    <div v-if="dupicateData" class="popup">
      <p>
        {{ alertFailed }}
      </p>
      <button @click="closePopup">
        닫기
      </button>
    </div>

  </div>
</template>

<script>

export default {

  data() {
    return {
      email: '',
      existingEmail: '',
      userName: '',
      password: '',
      passwordCheck: '',
      dupicateData: false, //유효성검사 변수
      alertFailed: '', //email, password 유효성 검사시 팝업 텍스트 변환 변수
    }
  },

  methods: {

    userEmailInput() {
      console.log("user Email Value ", this.email);
    },

    emailCheck() {
      console.log('userEmail: ', this.email)

      const response = this.$http.$get('')
      this.existingEmail = response.email

      if (this.email === this.existingEmail) {
        this.duplicateData = true
        this.alertFailed = '해당 이메일은 이미 사용중인 이메일입니다.'
      } else {
        this.duplicateData = false
      }
    },

    closePopup() {
      this.dupicateData = false
    },

    passwrodComfirmed() {
      if (this.password !== this.passwordCheck) {
        this.dupicateData = true
        this.alertFailed = '비밀번호가 다릅니다. 다시 확인해주세요.'
      } else {
        this.dupicateData = false
      }
    }
  },

  async signUp() {
    const email = this.email
    const userName = this.userName
    const passwordCheck = this.passwordCheck

    if (!this.dupicateData) {
      const response = this.$http.$post(
        '',
        {
          email,
          userName,
          passwordCheck
        }
      )
    }
  }
}
</script>

<style>
.popup {
  border: 1px solid #ccc;
  padding: 20px;
  background-color: #f9f9f9;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>