<template>
  <div id="app">
    <datetime-picker v-model="showPick" @getVal="getVal"></datetime-picker>
    <button @click="showPick = !showPick">隐藏/显示</button>
    <p>{{pickerValue}}</p>
  </div>
</template>

<script>
 import DatetimePicker from '../src/data-select/datetime-picker'

  export default {
    name: 'App',
    components: {DatetimePicker},
    data: function () {
      return {
        pickerValue: '',
        month: 1,
        showPick: false,
        day: 30
      }
    },
    methods: {
      getVal(e){
        this.pickerValue = e
      }
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
