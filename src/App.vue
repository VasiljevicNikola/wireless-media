<template>
  <div id="app">
    <myheader ></myheader>
    <router-view />
    <myfooter ></myfooter>
  </div>
</template>

<script>
import myheader from "./components/myheader"
import myfooter from "./components/myfooter"

export default {
  components:{
    myheader,
    myfooter
  }
}

</script>


<style>

</style>
