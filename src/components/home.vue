<template>
  <div class="home">
    <div class="wrapper">
      <div class="hero">

        <div class="">
          <div class="tackice">
            <img  class="" @click="" src="static/imgs/tackice.png" alt="">
          </div>
        </div>
        <div class="icon">
            <img  class="" @click="" src="static/imgs/icon.png" alt="">
            <div class="tekst">
              <h1>LOREM IPSUM DOLOR SIT</h1>
            </div>
        </div>
        <div class="dots">
          <div v-for="n in 3"class="dot">
          </div>
        </div>
      </div>
      <div class="tekst-mob">
        <div class="img">
          <img  class="" @click="" src="static/imgs/leftt.png" alt="">
        </div>
        <div class="img">
          <h1>LOREM IPSUM DOLOR SIT</h1>
        </div>

        <div class="img">
          <img  class="" @click="" src="static/imgs/right.png" alt="">
        </div>

      </div>

      <div class="main">
        <h2>WHO WE ARE</h2>
        <div class="first">
          <div class="slika">
            <img  class="" v-show="!kapa" @mouseover="kapa = true" src="static/imgs/kapa.png" alt="">
            <img  class="" v-show="kapa" @mouseleave="kapa = false" src="static/imgs/kapa-z.png" alt="">
          </div>
          <div class="opis">
            <p>Lorem ipsum</p>
            <br>
            <p class="opis-2">Lorem ipsum dolor sit amet,consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore</p>
            <button type="button" name="button">SHOW MORE</button>
          </div>

          <div class="slika">
            <img  class="" @click="" v-show="!like" @mouseover="like = true" src="static/imgs/like.png" alt="">
            <img  class="" @click="" v-show="like" @mouseleave="like = false" src="static/imgs/like-z.png" alt="">
          </div>
          <div class="opis">
            <p>Lorem ipsum</p>
            <br>
            <p class="opis-2">Lorem ipsum dolor sit amet,consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore</p>
            <button type="button" name="button">SHOW MORE</button>
          </div>
        </div>

          <h2>WHAT WE DO</h2>



        <div class="second">
          <div class="slika">
            <img  class="" @click="" v-show="!oblak" @mouseover="oblak = true" src="static/imgs/oblak.png" alt="">
            <img  class="" @click="" v-show="oblak" @mouseleave="oblak = false" src="static/imgs/oblak-z.png" alt="">
          </div>
          <div class="slika">
            <img  class="" @click="" v-show="!digitron" @mouseover="digitron = true" src="static/imgs/digitron.png" alt="">
            <img  class="" @click="" v-show="digitron" @mouseleave="digitron = false" src="static/imgs/digitron-z.png" alt="">
          </div>
          <div class="slika">
            <img  class="" @click="" v-show="!srce" @mouseover="srce = true" src="static/imgs/srce.png" alt="">
            <img  class="" @click="" v-show="srce" @mouseleave="srce = false" src="static/imgs/srce-z.png" alt="">
          </div>
          <div class="slika">
            <img  class="" @click="" v-show="!sat" @mouseover="sat = true" src="static/imgs/sat.png" alt="">
            <img  class="" @click="" v-show="sat" @mouseleave="sat = false" src="static/imgs/sat-z.png" alt="">
          </div>
        </div>
      </div>
    </div>


  </div>


</template>

<script>
export default {

  data () {
    return {
      kapa:false,
      like:false,
      sat:false,
      srce:false,
      oblak:false,
      digitron:false
    }
  }
}
</script>


<style lang="css" scoped>

</style>
