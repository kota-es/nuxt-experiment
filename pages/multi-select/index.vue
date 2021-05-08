<template>
  <div class="samaple__conntents">
    <div style="margin-top: 20px;">
      <div style="width: 50%; margin-left: 26%;">
        <h1 style="text-align: center;">Vue-multiselect</h1>
        <multiselect
          v-model="value"
          :multiple="true"
          :options="options"
        ></multiselect>
      </div>
    </div>
  </div>
</template>
<script>
import Vue from 'vue'
import Multiselect from 'vue-multiselect'

Vue.component('multiselect', Multiselect)
export default {
  components: { Multiselect },
  data() {
    return {
      value: null,
      options: ['list', 'of', 'options']
    }
  }
}
</script>
