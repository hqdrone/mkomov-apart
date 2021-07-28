<template>
  <app-main></app-main>
</template>
<script>
  import AppMain from '@/components/AppMain'

  export default {
    components: {
      AppMain
    },
    transition: 'home'
  }
</script>

<style>
  .home-enter-active, .home-leave-active { transition: opacity .5s; }
  .home-enter, .home-leave-active { opacity: 0; }
</style>
