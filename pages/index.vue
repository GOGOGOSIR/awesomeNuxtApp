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
          <NuxtLink class="nuxt-link-btn" to="/dynamicRoute/1">
            dynamicRoute/_slug/index
          </NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/dynamicRoute/2/comments">
            dynamicRoute/_slug/comments
          </NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/dynamicRoute/2/999">
            dynamicRoute/_slug/_list
          </NuxtLink>
        </div>
        <h2>嵌套路由</h2>
        <div class="linkWrapper">
          <NuxtLink class="nuxt-link-btn" to="/nested/normal">
            nested normal index
          </NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/nested/normal/1">
            nested normal _id
          </NuxtLink>
        </div>
        <h2>嵌套动态路由</h2>
        <div class="linkWrapper">
          <NuxtLink class="nuxt-link-btn" to="/nested/1">
            nested _dynamicNested index
          </NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/nested/1/2">
            nested _dynamicNested _sub
          </NuxtLink>
          <NuxtLink class="nuxt-link-btn" to="/nested/1/2/3">
            nested _dynamicNested _sub _id
          </NuxtLink>
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
  padding: 5px 15px;
  border: 1px solid #999;
  text-decoration: none;
  color: #333;
  border-radius: 4px;
  transition: all 0.3s;
}
.nuxt-link-btn:hover {
  color: #00c58e;
  border-color: #00c58e;
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
