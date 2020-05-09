<template>
  <div class="modal" :class="{ 'is-active': isActive }">
    <div class="modal-background" @click="closeModal"></div>
    <div class="modal-content">
      <div class="box">
        <component :is="window" />
      </div>
    </div>
    <button class="modal-close is-large" aria-label="close" @click="closeModal"></button>
  </div>
</template>

<script>
  import Inventory from './../Hud/Menu/Inventory'
  import Magic from './../Hud/Menu/Magic'
  import Map from './../Hud/Menu/Map'
  import Status from './../Hud/Menu/Status'

  export default {
    name: 'Modal',
    props: {
      isActive: {
        type: Boolean,
        default: false
      },
      window: {
        type: String,
        default: null
      }
    },
    components: {
      Inventory,
      Magic,
      Map,
      Status
    },
    methods: {
      closeModal() {
        this.$emit('close')
      }
    },
  }
</script>

<style lang="scss" scoped>

</style>