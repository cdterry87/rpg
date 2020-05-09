<template>
  <button class="button" :title="title">
    <span class="icon" v-if="icon">
      <i :class="icon"></i>
    </span>
  </button>
</template>

<script>
  export default {
    name: 'Button',
    props: {
      title: {
        type: String,
        default: null
      },
      icon: {
        type: String,
        default: null
      },
    },
  }
</script>

<style lang="scss" scoped>

</style>