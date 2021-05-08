<template>
  <div class="samaple__conntents">
    <div style="margin-top: 20px;">
      <h1>Vue-good-tableプラグインサンプル</h1>
    </div>
    <div style="margin-top: 20px;">
      <div style="width: 50%; margin-left: 23%;">
        <vue-good-table :columns="columns" :rows="rows" />
      </div>
    </div>
  </div>
</template>
<script>
import Vue from 'vue'
import vueGoodTable from 'vue-good-table'
import 'vue-good-table/dist/vue-good-table.css'

Vue.use(vueGoodTable)
export default {
  data() {
    return {
      columns: [
        {
          label: 'Name',
          field: 'name'
        },
        {
          label: '数値',
          field: 'value',
          type: 'number'
        },
        {
          label: '小数点',
          field: 'float',
          type: 'number'
        }
      ],
      rows: [
        { id: 1, name: 'John', value: 20, float: 20.1 },
        { id: 2, name: 'Jane', value: 24, float: 30.3 },
        { id: 3, name: 'Susan', value: 16, float: 20.5 },
        { id: 4, name: 'Chris', value: 55, float: 50.7 }
      ]
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
