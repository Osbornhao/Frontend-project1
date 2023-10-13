<script setup>
import HeadedParagraph from "@/components/HeadedParagraph.vue";
import Backgroundsvg from "@/components/icons/Iconbackgroundsvg.vue";
</script>

<template>
  <div class="grid">
    <div class="name">
      Guanyu
    </div>
 <HeadedParagraph class="left-text" header="333" paragraph="666"></HeadedParagraph>
  <HeadedParagraph class="right-text" header="222" paragraph="888"></HeadedParagraph>
    <div class="background">
      <Backgroundsvg class="background-svg">

      </Backgroundsvg>
    </div>
<!--    <Backgroundsvg class="background-svg">-->

<!--    </Backgroundsvg>-->
  </div>
</template>

<style scoped>
.grid{
  display: grid;
  grid-template-columns:1fr 2fr 1fr ;
  grid-template-rows: 1fr 5fr;
}
.left-text{
  grid-column-start: 1;
  grid-row-start: 2;
}
.right-text{
  grid-column-start: 3;
  grid-row-start: 2;
}
.name{
  display: flex;
  width: 1344px;
  height: 230px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  text-align: left;
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 96px;
  font-style: normal;
  font-weight: 700;
  line-height: 130%; /* 124.8px */
  grid-column-start: 1;
  grid-row-start: 1;
  grid-column-end: span 3;
}
.background{
  width: 30vw;
  height: 30vw;
  flex-shrink: 0;
  border-radius: 668px;
  background: #282828;
  grid-column-start: 2;
  grid-row-start: 2;
}
.background-svg{
  width:  28vw;
  height:  28vw;
  flex-shrink: 0;
  stroke-width: 20px;
  stroke: var(--color-text);
  grid-column-start: 2;
  grid-row-start: 2;
  display: block;
  margin: auto;
  //position: absolute;
  //bottom: 0;
}
</style>
