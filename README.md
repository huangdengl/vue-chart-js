# vue-chart-js

[![npm](https://img.shields.io/npm/v/vue-chart-js.svg)](https://www.npmjs.com/package/vue-chart-js)
[![npm](https://img.shields.io/npm/dt/vue-chart-js.svg)](https://www.npmjs.com/package/vue-chart-js)
[![npm](https://img.shields.io/npm/dm/vue-chart-js.svg)](https://www.npmjs.com/package/vue-chart-js)
[![npm](https://img.shields.io/npm/l/vue-chart-js.svg)](http://opensource.org/licenses/MIT)

[Chart.js](http://www.chartjs.org/) for [Vue](https://vuejs.org/).

## Installation

```sh
$ npm install vue-chart-js --save
```

## Usage

```vue
<template>
  <vue-chart type="bar" :data="chartData"></vue-chart>
</template>

<script>
import VueChart from 'vue-chart-js'

export default {
  name: 'App',

  components: {
    VueChart
  },

  data: () => ({
    chartData: {
        labels: ['Item 1', 'Item 2', 'Item 3'],
        datasets: [
            {
                label: 'Component 1',
                data: [10, 20, 30]
            },
            {
                label: 'Component 2',
                data: [20, 30, 40]
            }
        ]
    }
  }),
}
</script>

```

## Props
|Props|Description|Type|Required|
|-----|-----------|----|--------|
|type|Chart.js type|String|true|
|data|Chart.js datasets|Object|true|
|options|Chart.js options|Object|false|
|width|Chart width|Number|false|
|height|Chart height|Number|false|

## License

Vue-Chart-Js is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
