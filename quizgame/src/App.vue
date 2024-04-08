<template>
<body>
    
  <header-component></header-component>

  <center><h3>Select game mode</h3></center>

<center><div class="blocks__block">

  <div class="upper__blocks">
    <img class="image__in__block" src="@/assets/calculator.svg" alt="">
    <h3>TRENING</h3>
  </div>

  <div class="upper__blocks">
    <img class="image__in__block" src="@/assets/blizzard.svg" alt="">
    <h3>BATTLE</h3>
  </div>

</div>
</center>

<center>
  <div class="blocks__block">
    <div class="bottom__blocks">
      <h3>SOON</h3>
    </div>

    <div class="bottom__blocks">
      <h3>SOON</h3>
    </div>
  </div>
</center>
</body>
</template>

<script>
import HeaderComponent from "@/components/HeaderComponent.vue";
import "@/css/components/header.css";
import "@/css/components/home.css";

export default {
  name: 'App',
  components: {
    HeaderComponent
  }
}
</script>
