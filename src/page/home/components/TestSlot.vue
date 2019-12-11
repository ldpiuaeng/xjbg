<template>
  <div>
    <a :href="options">haha</a>
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: 'TestSlot',
  data () {
    return {
      options: 'http://www.lenovo.com'
    }
  }
}
</script>
<style scoped>
</style>
