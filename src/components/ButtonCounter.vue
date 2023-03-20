<template>
    <div>
      <button @click="sayHello()" >+</button>
      <button @click="sayH()" >-</button>
      <h1> You press button {{counter}} time</h1>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        counter: 0
      }
    },
    methods:
    {
      sayHello() {
        this.counter++
      },
      sayH() {
        this.counter--
      }
    },
  }
  </script>
  
  <style lang="scss" scoped>
  
  </style>