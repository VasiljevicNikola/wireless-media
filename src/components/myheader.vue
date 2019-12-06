<template lang="html">
  <div class="header">
    <div class="wrapper">
      <div class="logo">
        <router-link  to="/"> <img @click="scrollToTop()" src="static/imgs/logo.png" alt=""> </router-link>
      </div>
      <nav>
        <div id="navi" class="nav">
                <ul>
                  <li ><router-link  to="/"> HOME</router-link> / </li>
                  <li ><router-link to="/"> ABOUT US</router-link> / </li>
                  <li ><router-link  to="/"> OUR WORK</router-link> / </li>
                  <li ><router-link  to="/"> CONTACT</router-link></li>
                </ul>
        </div>
        <div class="search">
          <img  class="ser" @click="" src="static/imgs/search.png" alt="">
        </div>
      </nav>
      <div class="line">

      </div>

    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
</style>
