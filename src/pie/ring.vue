<template>
  <div class="ve-ring" :style="canvasStyle" ref="canvas"></div>
</template>

<script>
import echarts from '../echarts-base'
import { ring } from './pie'
import chartMixin from '../mixins'
export default {
  name: 'VeRing',
  mixins: [chartMixin],
  created () {
    this.chartHandler = ring
    this.echartsLib = echarts
  }
}
</script>
