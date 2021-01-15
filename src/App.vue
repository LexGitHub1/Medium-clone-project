<template>
  <div>
    <mcp-topbar />

    <router-view />
  </div>
</template>

<script>
import McpTopbar from '@/components/Topbar'
import {actionTypes} from '@/store/modules/auth'

export default {
  name: 'McpApp',
  components: {
    McpTopbar
  },
  mounted() {
    console.log('hello app')
    this.$store.dispatch(actionTypes.getCurrentUser)
  }
}
</script>
