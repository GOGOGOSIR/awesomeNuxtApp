<template>
  <div>
    component path: dynamicRoute/_slug/_list.vue
    <p>{{ routeParamsData }}</p>
  </div>
</template>

<script>
export default {
  data () {
    return {
      routeParamsData: {},
    }
  },
  created () {
    this.showLog()
  },
  methods: {
    showLog () {
      this.routeParamsData = this.$route.params
    },
  },
}
</script>
