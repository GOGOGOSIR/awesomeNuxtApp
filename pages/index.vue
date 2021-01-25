<template>
  <div class="container">
    <div>
      <Test />
      <Logo />
      <h1 class="title">awesomeNuxtApp</h1>
      <div class="links">
        <h2>静态路由</h2>
        <div class="linkWrapper">
          <NuxtLink class="nuxt-link-btn" to="/user">user index</NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/user/one">user one</NuxtLink>
        </div>
        <h2>动态路由</h2>
        <div class="linkWrapper">
          <NuxtLink class="nuxt-link-btn" to="/user">user index</NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/user/one">user one</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // layout: '404',
}
</script>

<style>
.linkWrapper {
  display: flex;
  justify-content: center;
}
.nuxt-link-btn {
  margin-right: 5px;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
