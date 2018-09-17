<template>
  <div class="radar_wrapper">
    <div id="chart"></div>
  </div>
</template>

<script>
import * as d3 from 'd3'
import RadarChart from "@/../static/RadarChart.js"
export default {
  name: "RadarCahrt",
  data () {
    return {
      width: 500,
      height: 500,
      fixData: [
        { area: "Central ", value: 80 },
        { area: "Kirkdale", value: 40 },
        { area: "Kensington ", value: 40 },
        { area: "Everton ", value: 90 },
        { area: "Picton ", value: 60 },
        { area: "Riverside ", value: 80 }
      ],
      chart: [
        [
          { area: "Central ", value: 80 },
          { area: "Kirkdale", value: 40 },
          { area: "Kensington ", value: 40 },
          { area: "Everton ", value: 90 },
          { area: "Picton ", value: 60 },
          { area: "Riverside ", value: 80 }
        ],
        [
          { area: "Central ", value: 40 },
          { area: "Kirkdale", value: 100 },
          { area: "Kensington ", value: 30 },
          { area: "Everton ", value: 10 },
          { area: "Picton ", value: 80 },
          { area: "Riverside ", value: 20 }
        ]
      ]
    }
  },
  methods: {
    drawChart () {
      const vm = this
      // let config = {
      //   w: this.width,
      //   h: this.height,
      //   maxValue: 100,
      //   levels: 5,
      //   ExtraWidthX: 180
      // }
      // RadarChart.draw("#chart", vm.chart, config)
      RadarChart.draw("#chart", vm.chart)
    }
  },
  mounted () {
    this.drawChart()
  }
}
</script>

<style lang="scss" scoped>
.radar_wrapper{
  width: 100%;
  overflow: hidden;
}
.levels{
  font-family: 'Courier New', Courier, monospace;
  font-size: 1em;
  font-weight: bold;
}
</style>
