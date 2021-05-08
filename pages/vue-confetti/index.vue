<template>
  <div class="samaple__conntents">
    <div style="margin-top: 20px;">
      <h1>vue-confettiプラグインサンプル</h1>
    </div>
    <div style="margin-top: 20px;">
      <button @click="start">Start</button>
      <button @click="stop">Stop</button>
      <button @click="test">Show some test</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    start() {
      this.$confetti.start()
    },
    stop() {
      this.$confetti.stop()
    },
    test() {
      this.$confetti.update({
        particles: [
          {
            type: 'heart'
          },
          {
            type: 'circle'
          }
        ],
        defaultColors: ['red', 'pink', '#ba0000']
      })
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
