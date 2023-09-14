<template>
  <div class="text-center m-4">
    <h2 class="text-3xl font-bold pb-0">С возвращением!</h2>
    <p>Децентрализованная сеть ждет вас</p>

    <div class="w-full">
      <form class="bg-white rounded px-8 pt-6 pb-8 mb-4">
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="password1">
            Пароль
          </label>
          <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="password1" type="password" placeholder="******************">
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="password2">
            Повторите пароль
          </label>
          <input class="shadow appearance-none border border-gray-600 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline" id="password2" type="password" placeholder="******************">
          <p class="text-red-500 text-xs italic">Пожалуйста придумайте пароль.</p>
        </div>
        <div class="flex items-center justify-between">
          <button @click="goNext" type="button" class="uppercase bg-cyan-800 hover:bg-gr-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline">
            Продолжить
          </button>
          <a class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800" href="#">
            Сбросить все?
          </a>
        </div>
      </form>
      <p class="text-center text-gray-500 text-xs">
        &copy;2023 SmartHoldem Platform
      </p>
    </div>

    <RouterLink to="/about">О кошельке</RouterLink>
  </div>
</template>


<script>
export default {
  name: "home",
  methods: {
    async goNext() {
      this.$router.push('/accounts')
    }
  }
}
</script>

<style>
.logo {
  text-align: center;
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
