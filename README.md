# simple-dateselect-vue

> a simple Date selection component for vue

 ![image](https://raw.githubusercontent.com/mshaital/simple-dateselect-vue/master/src/assets/20190202110036.png)

    一个简单的vue 日期选择组件 只能选择日期
    由于项目特殊要求重写了他人的插件
    原版是用jquery写的改成vue组件,改写很多基本上算是重写了
    扩展性不强 颜色大小位置都能不能改 需要的话自己改源码吧 个性化需求那么多不可能全满足

## Installing
$ npm install simple-dateselect-vue --save

import SimpleDateselectVue from 'simple-dateselect-vue'

## Examples
```javascript
<simple-dateselect-vue v-model="showPick" @getVal="getVal"></simple-dateselect-vue>
```

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

