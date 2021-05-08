<script>
import { Line } from 'vue-chartjs'
export default {
  extends: Line,
  props: {
    chartdata: {
      type: Object
    },
    options: {
      type: Object,
      default: () => ({
        responsive: true,
        maintainAspectRatio: false
      })
    }
  },
  mounted() {
    this.renderChart(this.chartdata, this.options)
  }
}
</script>
