# simple-dateselect-vue

> a simple Date selection component for vue

 ![image](https://github.com/mshaital/simple-dateselect-vue/blob/master/src/assets/20190202110036.png)
## Installing

$ npm install simple-dateselect-vue --save

import SimpleDateselectVue from 'simple-dateselect-vue'

``` bash
# Examples
<datetime-picker v-model="showPick" @getVal="getVal"></datetime-picker> <br>

showPick 控制显示隐藏
getVal 事件得到选择的数据

## API

### Props

| Name        | Type     | Description            | Default                  |
| :-----      | :------- | :----------------------| :----------------------- |
| showPick    | Boolean  | show or hidden.        | false                    |
| startYear   | Number   | Which year to start    | 1900                     |
| endYear     | Number   | Which year to end      | 2100                     |
| defaultDate | Date     | default date to show   | new Date()               |

### Events

| Name    | Description |
| :-----  | :---------- |
| getVal  |  get value  |
