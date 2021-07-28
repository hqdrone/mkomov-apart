<template>
  <section class="reg">
    <div class="container">
      <h2 class="reg__h2 h2">Регистрация</h2>
      <div class="reg__form">
        <form @submit.prevent="onSubmit" v-if="!loader">
          <label>Адрес эл. почты
            <input type="email" v-model="form.email"/>
          </label>
          <label>Пароль
            <input type="password" v-model="form.password"/>
          </label>
          <label>Город
            <select v-model="form.city">
              <option v-for="city in cities" :value="city.id" >{{city.name}}</option>
            </select>
          </label>
          <label>
            <input type="checkbox" v-model="form.accept"/>Согласен с условиями обработки перс. данных
          </label>
          <div class="reg__button button">
            <button :disabled="!isValid">Зарегистрироваться</button>
          </div>
        </form>
        <div class="reg__loader" v-if="loader">
          <svg viewBox="25 25 50 50">
            <circle cx="50" cy="50" r="20"></circle>
          </svg>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

  export default {
    data() {
      return {
        cities: [],
        form: {
          email: '',
          password: '',
          city: '',
          accept: false
        },
        loader: false
      }
    },
    methods: {
      async getCities() {
        this.cities = await this.$axios.$get('https://61010c051d56e10017394d50.mockapi.io/api/cities')
      },
      async onSubmit() {
        try {
          this.loader = true
          const user = {
            email: this.form.email,
            password: this.form.password,
            cityId: this.form.city
          }
          await this.$axios.$post('https://61010c051d56e10017394d50.mockapi.io/api/users', user)
          this.$router.push('success')
          this.loader = false
        } catch (e) {
          console.error(e)
        }
      }
    },
    computed: {
      isValid() {
        return this.form.email && this.form.password && this.form.city && this.form.accept === true
      }
    },
    created() {
      this.getCities()
    }
  }
</script>
