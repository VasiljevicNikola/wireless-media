<template lang="html">
  <header>
    <div class="wrapper">
      <div class="logo">
        <router-link  to="/"> <img @click="scrollToTop()" src="static/imgs/logo.png" alt=""> </router-link>
      </div>
      <nav id="navi">
        <div  class="nav">
                <ul class="laptop">
                  <router-link  to="/"><li class="home"> HOME / </li></router-link>
                  <router-link to="/"><li class="about"> ABOUT US / </li></router-link>
                  <router-link  to="/"> <li class="work">OUR WORK / </li></router-link>
                  <router-link  to="/"><li class="contact"> CONTACT</li></router-link>
                </ul>
                <div class="tablet">
                  <router-link  to="/"><img  class="ser" v-show="!kucica" @mouseover="kucica = true"  src="static/imgs/kucica.png" alt=""></router-link>
                  <router-link to="/"><img  class="ser" v-show="kucica" @mouseover="kucica = true"  src="static/imgs/kucica-z.png" alt=""></router-link>

                  <router-link  to="/"><img  class="ser" v-show="!znak" @mouseover="znak = true"  src="static/imgs/znak.png" alt=""></router-link>
                  <router-link  to="/"><img  class="ser" v-show="znak" @mouseover="znak = true"  src="static/imgs/znak-z.png" alt=""></router-link>

                  <router-link  to="/"><img  class="ser" v-show="!kapa" @mouseover="kkapa = true"  src="static/imgs/kapa.png" alt=""></router-link>
                  <router-link to="/"><img  class="ser" v-show="kapa" @mouseover="kapa = true"  src="static/imgs/kapa-z.png" alt=""></router-link>

                  <router-link  to="/"><img  class="ser" v-show="!pismo" @mouseover="pismo = true"  src="static/imgs/pismo.png" alt=""></router-link>
                  <router-link  to="/"><img  class="ser" v-show="pismo" @mouseover="pismo = true"  src="static/imgs/pismo-z.png" alt=""></router-link>
                </div>
        </div>
        <div class="search">
          <img  class="ser" v-show="!search" @mouseover="search = true"  src="static/imgs/search.png" alt="">
          <img  class="ser" v-show="search" @mouseleave="search = false" @click="findsomething($event)" src="static/imgs/search-z.png" alt="">
          <div v-if="find" class="search-input">
            <input type="text" name="" value="" v-model="searching">
          </div>
        </div>
      </nav>
      <div v-if="find" class="search-input">
        <input type="text" name="" value="" v-model="searching">
      </div>
      <nav class="mob">
        <div class="icon-mob">
            <p @click="mob=!mob"><i class="fa fa-bars"></i> </p>
          </div>
          <div v-if="mob" id="navmob" class="animated slideInDown">
                <ul>
                  <router-link  to="/"><li @click="mob = false" class="home"> HOME</li></router-link>
                  <router-link to="/"><li @click="mob = false" class="about"> ABOUT US</li></router-link>
                  <router-link  to="/"> <li @click="mob = false" class="work">OUR WORK</li></router-link>
                  <router-link  to="/"><li @click="mob = false" class="contact"> CONTACT</li></router-link>
                </ul>
        </div>
        <div class="search">
          <img  class="ser" v-show="!search" @mouseover="search = true"  src="static/imgs/search.png" alt="">
          <img  class="ser" v-show="search" @mouseleave="search = false" @click="findsomething($event)" src="static/imgs/search-z.png" alt="">

        </div>
        <div v-if="find" class="search-input">
          <input type="text" name="" value="" v-model="searching">
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
      mob:false,
      find:false,
      search:false,
      searching:"",
      kucica:false,
      znak:false,
      kapa:false,
      pismo:false
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
