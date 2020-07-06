<template>
  <div class="home">
    <Twitter/>
  </div>
</template>

<script>
// @ is an alias to /src
import Twitter from '@/components/Twitter.vue'

export default {
  name: 'Home',
  components: {
    Twitter
  }
}
</script>
