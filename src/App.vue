<template>
  <div id="app">
    <app-topbar />
    <router-view />
  </div>
</template>

<script>
import appTopbar from '@/components/Topbar.vue'

export default {
  name: 'App',
  components: {
    appTopbar,
  },
}
</script>
