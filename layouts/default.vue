<template>
  <div class="app">
    <the-header></the-header>
    <nuxt></nuxt>
    <the-footer></the-footer>
  </div>
</template>

<script>
  import TheHeader from '@/components/TheHeader'
  import TheFooter from '@/components/TheFooter'

  export default {
    components: {
      TheHeader,
      TheFooter
    }
  }
</script>
