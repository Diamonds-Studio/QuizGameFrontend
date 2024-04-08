<template>
  
  <div class="Home">
  <div class="logoHome">
    <img src="QuizGameFrontend/quiz-game/src/img/home/LogoFile.jpg" alt="">
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
  <img src="QuizGameFrontend/quiz-game/src/img/home/Discord.png" alt="">
  <p>Sigh in with Discord</p>
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


