<script setup>
import Arrow from "@/components/icons/Iconarrow.vue";
</script>

<template>
<div class="Rectangle1">
 <Arrow class="arrow">
 </Arrow>
  <div class="size">
    Let’s work together
  </div>
</div>
</template>

<style scoped>
.Rectangle1 {
  height: 90px;
  border-radius: 30px;
  border: 1px solid #F3F3F3;
  position: relative;
  width: 400px;
}

.size {
  font-size: 48px;
  font-style: normal;
  font-weight: 300;
  line-height: 130%; /* 62.4px */
  letter-spacing: -4.32px;
  display: flex;
  width: 384px;
  height: 37px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  padding: 60px 0 1rem 1rem;
}

.arrow {
  stroke-width: 3px;
  stroke:var(--color-text);
  width: 52px;
  height: 37px;
  flex-shrink: 0;
  position: absolute;
  right: 0;
  margin: 10px 5px 1rem 1rem;;
}
</style>