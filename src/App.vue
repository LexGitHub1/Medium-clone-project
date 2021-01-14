<template>
  <div>
    <mcp-topbar />

    <router-view />
  </div>
</template>

<script>
import McpTopbar from '@/components/Topbar'

export default {
  name: 'McpApp',
  components: {
    McpTopbar
  }
}
</script>
