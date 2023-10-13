<script setup>

</script>

<template>
  <div class="homepage-grid">
  <div class="left-group">
    <img  class="homepage-img" src="../assets/IMG_1783_副本.JPG" alt="">
    <div class="homepage-t">
     金门大桥
    </div>
  </div>
  <div class="right-group">
    <div class="homepage-t right-t">
      金门大桥2金门大桥2
    </div>
    <img class="homepage-img" src="../assets/IMG_1783_副本.JPG" alt="">
    <div class="homepage-t right-t">
      金门大桥3金门大桥3
    </div>
  </div>
  </div>
</template>

<style scoped>
.homepage-img {
  width: 90%;
  height: auto;
}

.homepage-t {
  color: #FFF;
  font-feature-settings: 'clig' off, 'liga' off;
  font-family: Inter;
  font-size: 24px;
  font-style: normal;
  font-weight: 700;
  line-height: 130%; /* 31.2px */
}

.right-t {
  //margin:1em 0;
}

.homepage-grid {
  display: grid;
  grid-template-columns: 1fr 3fr;
  column-gap: 1em;
  transform: rotate(-15deg);
  width: 80%;
  height: auto;
  margin-left: 6rem;
  margin-top: -15rem;
}

</style>