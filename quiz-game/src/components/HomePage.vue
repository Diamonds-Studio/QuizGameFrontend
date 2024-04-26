<template>
  <div class="Home">
    <div class="logoHome">
      <img src="../img/home/Logo.png" alt="" />
    </div>
    <div class="logoText">
      <p>Where Equations Clash and Algorithms Due</p>
    </div>
    <div class="imgefotoMeneger">
      <div class="imgefoto"></div>
    </div>
    <div class="RegisterDiscordMeneger">
      <button class="RegisterDiscord" @click="redirectToDiscordAuth">
        <a
          href="https://discord.com/oauth2/authorize?client_id=1227686332260946000&response_type=code&redirect_uri=https%3A%2F%2Fquiz-game-three-cyan.vercel.app%2F&scope=identify"
        >
          <img src="../img/home/Discord.png" alt="" />
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
import "@/assets/css/PagesStyles/home.css";

export default {
  name: "HomePage",
  props: {
    msg: String,
  },
  methods: {
    redirectToDiscordAuth() {
      window.location.href =
        "https://discord.com/oauth2/authorize?client_id=1227686332260946000&response_type=code&redirect_uri=https%3A%2F%2Fquiz-game-three-cyan.vercel.app%2F&scope=identify";
      // Перенаправление на страницу MainPage.vue после успешной аутентификации на Discord
      // Здесь вы можете добавить логику для проверки успешной регистрации
      // Например, используя callback URL или другие методы аутентификации
      window.location.href = "./components/MainPage.vue";
    },
  },

  created() {
    try {
      const currentUrl = window.location.href;

      const url = new URL(currentUrl);

      const params = new URLSearchParams(url.search);

      let authCode = params.get("code");

      console.log(authCode);
    } catch (error) {
      console.error("Auth Code error:", error);
    }
  },
};
</script>
<style >
body {
  background-color: #1c1c1c;
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
}
</style>


