<template>
  <div class="samaple__conntents">
    <diV style="margin-top: 20px;">
      <h1>nuxt-i18nプラグインサンプル</h1>
    </diV>
    <diV style="margin-top: 20px;">
      {{ $t('message') }}
    </diV>
    <div>
      <nuxt-link :to="switchLocalePath('en')">English</nuxt-link>
    </div>
    <div>
      <nuxt-link :to="switchLocalePath('ja')">japanese</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0
    }
  }
}
</script>

<style>
.samaple__conntents {
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
