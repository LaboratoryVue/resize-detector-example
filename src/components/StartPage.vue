<template>
  <div class="start">
    <section ref="block" class="block"></section>
  </div>
</template>

<script>
import { addListener, removeListener } from 'resize-detector'

export default {
  name: 'StartPage',
  methods: {
    onEventRise() {
      addListener(this.$refs.block, () => console.log(`resize start`))
    },
    onEventDown() {
      removeListener(this.$refs.block, () => console.log(`resize down`))
    }
  }
}
</script>

<style scoped lang="scss">
.block {
  width: 100%;
  min-width: 100%;
}
</style>
