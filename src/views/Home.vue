<template>
  <div v-once class="home">
    <HelloWorld :msg="msg"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  data () {
    return {
      msg: require('@/assets/content.json').headline
    }
  },
  components: {
    HelloWorld
  }
}
</script>
