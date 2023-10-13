<script setup>
import {ref} from "vue";
import Img from "../assets/IMG_1783_副本.JPG"
import Img1 from "../assets/IMG_8913.JPG"
const sites = ref([
  { image:Img },
  { image:Img1 },
  {image:Img }
])
</script>

<template>
<div class="thumbnail-list">
  <div class="thumbnail" v-for="site in sites">
   <img class="thumbnail-img" :src="site.image">
  </div>
</div>
</template>

<style scoped>
.thumbnail-list{
  width: 80%;
}
.thumbnail{
  width: 240px;
  height: 150px;
  flex-shrink: 0;
  border-radius: 20px;
  margin-bottom: 1rem;
}
.thumbnail-img{
  width: 240px;
  height: 150px;
  flex-shrink: 0;
  border-radius: 20px;
}

</style>