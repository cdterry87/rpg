<template>
  <div id="menu" class="buttons">
    <Button
      title="Inventory"
      @click.native="open('Inventory')"
      icon="fas fa-th"
    />
    <Button
      title="Map"
      @click.native="open('Map')"
      icon="fas fa-map"
    />
    <Button
      title="Magic"
      @click.native="open('Magic')"
      icon="fas fa-hand-sparkles"
    />
    <Button
      title="Status"
      @click.native="open('Status')"
      icon="fas fa-user"
    />
    <Modal
      :is-active="modal"
      :window="window"
      @close="close"
    />
  </div>
</template>

<script>
  import Button from './../Utilities/Button'
  import Modal from './../Utilities/Modal'

  export default {
    name: 'Menu',
    components: {
      Button,
      Modal
    },
    data() {
      return {
        modal: false,
        window: null,
      }
    },
    methods: {
      open(window) {
        this.modal = true
        this.window = window
      },
      close() {
        this.modal = false
        this.window = null
      }
    },
  }
</script>

<style lang="scss" scoped>
  #menu {
    width: 100%;
    display: flex;
    justify-content: space-evenly;
  }
</style>