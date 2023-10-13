<script setup>
import Homepage from "@/components/Homepage.vue";
import Worktogether from "@/components/Worktogether.vue";
</script>
<template>
  <div class="home-wrapper">
  <div class="name">
    Guanyu
  </div>
  <div class="homepage-img">
    <Homepage>
    </Homepage>
  </div>
    <Worktogether class="home-button"></Worktogether>
  </div>

</template>

<style scoped>
.name {
  display: flex;
  width: 500px;
  height: 150px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  text-align: center;
  font-size: 100px;
  font-style: normal;
  font-weight: 700;
  line-height: 130%; /* 195px */
}
.home-wrapper {
  //display:grid;
  //grid-template-rows: 1fr 3fr ;
}

@media (min-width: 1024px) {
  .homepage-img {
    height: 100vh;
    width: 1200px;
    //overflow: hidden;
    display: flex;
    align-items: center;
    //transform: translate(8rem,0);
  }
  .home-button {
    transform: translate(0,-15rem) scale(0.7);
  }
}
</style>