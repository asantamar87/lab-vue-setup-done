<template>
  <header>
    <img
      alt="Vue logo"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    />
  </header>
  <Composition/>

  <div class="wrapper">
    <HelloWorld msg="Lab Vue 001 - Vue Setup" />
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <router-link to="/about-page">About Page</router-link>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/wu-tang">Wu Tang</RouterLink>
      <a href="/wu-tang">Wu Tang Using an aTag</a>
      <RouterLink to="/about-page"
        >About Page with diff folder structure</RouterLink
      >
    </nav>
  </div>

</template>


<script setup>
import Composition from './components/Composition.vue';

</script>


<style scoped>

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}


nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
