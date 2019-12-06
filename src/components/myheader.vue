<template lang="html">
  <header>
    <div class="wrapper">
      <div class="logo">
        <router-link  to="/"> <img @click="scrollToTop()" src="static/imgs/logo.png" alt=""> </router-link>
      </div>
      <nav>
        <div id="navi" class="nav">
                <ul>
                  <router-link  to="/"><li class="home"> HOME / </li></router-link>
                  <router-link to="/"><li class="about"> ABOUT US / </li></router-link>
                  <router-link  to="/"> <li class="work">OUR WORK / </li></router-link>
                  <router-link  to="/"><li class="contact"> CONTACT</li></router-link>
                </ul>
        </div>
        <div class="search">
          <img  class="ser" v-show="!search" @mouseover="search = true"  src="static/imgs/search.png" alt="">
          <img  class="ser" v-show="search" @mouseleave="search = false" @click="findsomething($event)" src="static/imgs/search-z.png" alt="">
          <div v-if="find" class="search-input">
            <input type="text" name="" value="" v-model="searching">
          </div>
        </div>
      </nav>

      <div class="line">

      </div>

    </div>
  </header>
</template>

<script>
export default {
  data(){
    return{
      find:false,
      search:false,
      searching:""
    }

  },
  methods:{
    findsomething(e){
      this.find= !this.find
      e.stopPropagation()
    }
  }
}
</script>

<style lang="css" scoped>
</style>
