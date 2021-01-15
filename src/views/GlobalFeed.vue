<template>
  <div class="home-page">
    BANNER
    <div class="container page">
      <div class="row">
        <div class="col-md-9">
          <mcp-feed :api-url="apiUrl" />
        </div>
        <div class="col-md-3">
          POPULAR TAGS
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import McpFeed from '@/components/Feed'
export default {
  name: 'McpGlobalFeed',
  components: {
    McpFeed
  },
  data() {
    return {
      apiUrl: '/articles'
    }
  }
}
</script>
