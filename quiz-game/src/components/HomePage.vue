<template>
  
  <div class="Home">
  <div class="logoHome">
    <img src="../img/home/Logo.png" alt="">
  </div>
  <div class="logoText">
    <p>Where Equations Clash and Algorithms Due</p>

  </div>
  <div class="imgefotoMeneger">
  <div class="imgefoto">

  </div>
</div>
<div class="RegisterDiscordMeneger">
  <button class="RegisterDiscord">
    <a href="https://discord.com/oauth2/authorize?client_id=1227686332260946000&response_type=code&redirect_uri=https%3A%2F%2Fquiz-game-three-cyan.vercel.app%2F&scope=identify" target="_blank">
      <img src="../img/home/Discord.png" alt="">
      <p>Sign in with Discord</p>
    </a>
  </button>
</div>
<div class="MadeTextMeneger">
<div class="Madetext">
  <p>Made in exchange for the abolition of taxes.</p>
  <p>MathBattle</p>
</div>
</div>
  </div>
</template>

<script>
import '@/assets/css/PagesStyles/home.css'

export default {
  name: 'HomePage',
  props: {
    msg: String
  }
}


</script>
<style >
body {
  background-color:#1C1C1C;
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
}
</style>


