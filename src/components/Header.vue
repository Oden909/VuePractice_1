<template>
  <header>
    <a href="/">
      <img :src="image" alt="Logo"/>
    </a>
    <nav>
      <a href="/">About</a>
      <a href="/">Work</a>
      <a href="/">Contact</a>
    </nav>
  </header>
</template>

<script>
    export default {

    }
</script>

<style scoped>
      header {
    display: flex;
    justify-content: space-between;
    padding: 40px;
    margin-bottom: 40px;
  }

  nav {
    display: flex;
    gap: 20px;
  }
</style>