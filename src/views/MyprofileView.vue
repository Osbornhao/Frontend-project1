<script setup>
import HeadedParagraph from "@/components/HeadedParagraph.vue";
import ThumbnailList from "@/components/ThumbnailList.vue";
</script>

<template>
  <div class="grid">
    <div class="name">
      Guanyu
    </div>
    <ThumbnailList class="thumbnail-list"></ThumbnailList>
    <img class="img" src="../assets/IMG_1783_副本.JPG" alt="">
<HeadedParagraph class="text" paragraph="555" header="666"></HeadedParagraph>
  </div>
</template>

<style scoped>
.grid{
  display: grid;
  grid-template-columns:1fr 2fr 6fr ;
  grid-template-rows: 1fr 1fr;
  height: 100vh;
  //align-items: end;
}
.text{
  width: 784px;
  height: 177px;
  flex-shrink: 0;
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 24px;
  font-style: normal;
  font-weight: 500;
  line-height: 130%; /* 31.2px */
  grid-column-start: 3;
  grid-row-start: 2;
}
.name{
  width: 145px;
  height: 147px;
  flex-shrink: 0;
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 48px;
  font-style: normal;
  font-weight: 500;
  line-height: 90%; /* 43.2px */
  grid-column-start: 1;
  grid-row-start: 1;
}
.img{
  width: 500px;
  height: 300px;
  flex-shrink: 0;
  grid-column-start: 3;
  grid-row-start: 1;
  //position: absolute;
  //bottom: -1fr;
  align-self: flex-end;
}
.thumbnail-list{
  grid-column-start: 2;
  grid-row-start: 1;
  grid-row-end:3;
  margin: 1rem 1rem 1rem 2rem;
}
</style>