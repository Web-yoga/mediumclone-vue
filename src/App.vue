<template>
  <div id="app">
    <app-topbar />
    <router-view />
  </div>
</template>

<script>
import appTopbar from '@/components/Topbar.vue'
import {actionsTypes} from '@/store/modules/auth'

export default {
  name: 'App',
  components: {
    appTopbar,
  },
  mounted() {
    this.$store.dispatch(actionsTypes.getCurrentUser)
  },
}
</script>
