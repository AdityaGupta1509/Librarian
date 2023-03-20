<template>
    <div>
      <input type="text" placeholder="First name" v-model="fname">
      <input type="text" placeholder="First name" v-model="lname">
      <h1>Welcome {{fullName}}</h1>
    </div>
  </template>
  
  <script>
    export default {
      data() {
        return {
          fname: '',
          lname: '',
          fullName: ''
        }
      },
      watch: {
        fname(newValue, oldValue) {
          this.fullName = newValue+' '+this.lname
        },
        lname(newValue, oldValue) {
          this.fullName = this.fname+' '+newValue
        },
      },
    }
  </script>
  
  <style lang="scss" scoped>
  
  </style>