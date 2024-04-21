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
    <a href="https://discord.com/oauth2/authorize?client_id=1227686332260946000&response_type=code&redirect_uri=https%3A%2F%2Fquiz-game-three-cyan.vercel.app%2F&scope=identify" >
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
// Функция для установки куки
function setCookie(name, value, days) {
    var expires = "";
    if (days) {
        var date = new Date();
        date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
        expires = "; expires=" + date.toUTCString();
    }
    document.cookie = name + "=" + (value || "") + expires + "; path=/";
}

// Предположим, что после успешной регистрации через Discord у вас есть токен доступа
var discordAccessToken = "your_access_token_here";

// Устанавливаем куки с токеном доступа на, скажем, 30 дней
setCookie("discord_access_token", discordAccessToken, 30);
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


