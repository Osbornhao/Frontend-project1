<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Showmore from "@/components/Showmore.vue";
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/Contactpage" class="nav-item">Contact page</RouterLink>
        <RouterLink to="/Myprofile" class="nav-item">My profile</RouterLink>
        <RouterLink to="/Whoami" class="nav-item">Who am i</RouterLink>
        <RouterLink to="/" class="nav-item">Home</RouterLink>
<!--        <RouterLink to="/Whoami" class="nav-item">Who am i</RouterLink>-->
<!--        <RouterLink to="/Myprofile" class="nav-item">My profile</RouterLink>-->
<!--        <RouterLink to="/Contactpage" class="nav-item">Contact page</RouterLink>-->
      </nav>
    </div>
    <Showmore></Showmore>

  </header>

  <RouterView />
</template>

<style scoped>
header {
  position: static;
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  //width: 100%;
  //font-size: 12px;
  //text-align: center;
  //margin-top: 2rem;
  font-size: 1rem;
  font-weight: bold;
  text-align: center;
  z-index:200; /* high z index so other content scrolls underneath */
  background-color: var(--color-background);
}

nav a.router-link-exact-active {
  color: var(--color-text);
  text-transform: uppercase;
  text-shadow: 0px 0px 10px #FFF;
}

nav a.router-link-exact-active:hover {
  text-shadow: 0px 0px 10px #FFF;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    //padding-right: calc(var(--section-gap) / 2);
    width: 6rem;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    max-width: 6rem;
  }

  .nav-item {
    transform: rotate(-90deg);
  }

  nav a {
    display: block;
    padding: 3rem 0;
    width: 120px;
    position: static;
  }
}
</style>
