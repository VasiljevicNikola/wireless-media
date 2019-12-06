<template lang="html">
  <div class="wrapper">
  <footer class="footer">
<div class="left-pics">
  <div class="pics">
    <img  class="" @click="" v-show="!face" @mouseover="face = true" src="static/imgs/face.png" alt="">
    <img  class="" @click="" v-show="face" @mouseleave="face = false" src="static/imgs/face-z.png" alt="">
  </div>
  <div class="pics">
    <img  class="" @click="" v-show="!twiter" @mouseover="twiter = true" src="static/imgs/twiter.png" alt="">
    <img  class="" @click="" v-show="twiter" @mouseleave="twiter = false" src="static/imgs/twiter-z.png" alt="">
  </div>
  <div class="pics">
    <img  class="" @click="" v-show="!pismo" @mouseover="pismo = true" src="static/imgs/pismo.png" alt="">
    <img  class="" @click="" v-show="pismo" @mouseleave="pismo = false" src="static/imgs/pismo-z.png" alt="">
  </div>
</div>



      <nav>
        <div id="navi" class="nav">
                <ul>
                  <router-link  to="/"><li class="home"> HOME  </li></router-link>
                  <router-link to="/"><li class="about"> ABOUT US  </li></router-link>
                  <router-link  to="/"> <li class="work">OUR WORK  </li></router-link>
                  <router-link  to="/"><li class="contact"> CONTACT </li></router-link>
                </ul>
        </div>
      </nav>
      <div class="right-pics">
      <div class="pics">
        <img  class="" @click="" v-show="!strelica" @mouseover="strelica = true" src="static/imgs/strelica.png" alt="">
        <img  class="" @click="" v-show="strelica" @mouseleave="strelica = false" src="static/imgs/strelica-z.png" alt="">
      </div>
      </div>



  </footer>
  </div>
</template>

<script>
export default {
  data () {
    return {
      face:false,
      twiter:false,
      pismo:false,
      strelica:false
    }
  }
}
</script>

<style lang="css" scoped>
</style>
