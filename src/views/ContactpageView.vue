<script setup>
import Address from "@/components/icons/Iconaddress.vue";
import Phonenumber from "@/components/icons/Iconphonenumber.vue";
import Email from "@/components/icons/Iconemail.vue";
</script>

<template>
  <div class="grid">
    <div class="header">
      <div style="opacity: 0.25;">
      Contact
      </div>
      <div style="opacity: 0.50;">
        Contact
      </div>
      <div style="opacity: 0.75;">
        Contact
      </div>
      <div style="opacity: 1;">
        Contact
      </div>
    </div>

    <div class="name">
      Guanyu
    </div>
    <Address class="address-svg">
    </Address>
    <Phonenumber class="number-svg">
    </Phonenumber>
    <Email class="email-svg">
    </Email>
    <div class="address-text">
      4255 NW Duniway
    </div>
    <div class="number-text">
      541-123123
    </div>
    <div class="email-text">
      123@gmail.com
    </div>
  </div>
</template>

<style scoped>
.grid{
  display: grid;
  grid-template-columns:35% auto;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
  //grid-column-gap: 5rem;
  height: 100vh;

}
.name{
  display: flex;
  width: 500px;
  height: 100px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  text-align: center;
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 80px;
  font-style: normal;
  font-weight: 300;
  line-height: 130%; /* 195px */
  grid-column-start: 1;
  grid-row-start: 2;
  grid-column-end: 3;
  justify-self:center;
}
.header{
  display: flex;
  width: 800px;
  height: 230px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: rgba(255, 255, 255, 0.75);
  text-align: center;
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 96px;
  font-style: normal;
  font-weight: 400;
  line-height: 35%; /* 90.72px */
  letter-spacing: 58.56px;
  grid-column-start: 1;
  grid-row-start: 1;
  grid-column-end: 3;
  justify-self:center;
}
.address-svg{
  width: 100px;
  height: 100px;
  flex-shrink: 0;
  stroke-width: 10px;
  stroke: var(--color-text);
  grid-column-start: 1;
  grid-row-start: 3;
  justify-self: end;
  //margin-right: 3rem;
}
.number-svg{
  width: 128px;
  height: 128px;
  flex-shrink: 0;
  stroke-width: 10px;
  stroke: var(--color-text);
  grid-column-start: 1;
  grid-row-start: 4;
  justify-self: end;
}
.email-svg{
  width: 128px;
  height: 128px;
  flex-shrink: 0;
  stroke-width: 10px;
  stroke: var(--color-text);
  grid-column-start: 1;
  grid-row-start: 5;
  justify-self: end;
}
.address-text{
  display: flex;
  //width: 700px;
  height: 142px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 40px;
  font-style: normal;
  font-weight: 400;
  line-height: 94.5%; /* 37.8px */
  grid-column-start: 2;
  grid-row-start: 3;
  margin-left: 5rem;
}
.number-text{
  display: flex;
  //width: 700px;
  height: 142px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 40px;
  font-style: normal;
  font-weight: 400;
  line-height: 94.5%; /* 37.8px */
  grid-column-start: 2;
  grid-row-start: 4;
  margin-left: 5rem;
}
.email-text{
  display: flex;
  //width: 700px;
  height: 142px;
  flex-direction: column;
  justify-content: center;
  flex-shrink: 0;
  color: var(--color-text);
  font-feature-settings: 'clig' off, 'liga' off;
  font-size: 40px;
  font-style: normal;
  font-weight: 400;
  line-height: 94.5%; /* 37.8px */
  grid-column-start: 2;
  grid-row-start: 5;
  margin-left: 5rem;
}

</style>