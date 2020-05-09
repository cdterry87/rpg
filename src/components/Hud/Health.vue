<template>
  <div id="health">
    <progress class="progress is-danger" value="100" max="100">100</progress>
  </div>
</template>

<script>
  export default {
    name: 'Health'
  }
</script>

<style lang="scss" scoped>
  #health {
    display: flex;
    align-items: center;
    width: 100%;
  }
</style>