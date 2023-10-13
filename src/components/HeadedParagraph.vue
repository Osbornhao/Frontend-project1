<script setup>
defineProps({
  header: {
    type: String,
    required: true
  },
  paragraph: {
    type: String,
    required: true
  }
})
</script>

<template>
<div class="size">
  <div class="header">
    {{ header }}
  </div>
  <div class="paragraph">
    {{ paragraph }}
  </div>

</div>
</template>

<style scoped>
.size{
  width: 270px;
  height: 533px;
  flex-shrink: 0;
}
.header{
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 36px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%; /* 54px */
}
.paragraph{
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 24px;
  font-style: normal;
  font-weight: 500;
  line-height: 150%;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

</style>