<template>
  <div id="hud" class="footer">
    <div class="container">
      <div class="columns is-multiline">
        <div class="column is-one-third">
          <Experience />
        </div>
        <div class="column is-one-third">
          <Health />
        </div>
        <div class="column is-one-third">
          <Menu />
        </div>
        <div class="column is-one-third">
          <Gold />
        </div>
        <div class="column is-one-third">
          <Mana />
        </div>
        <div class="column is-one-third">
          <Spells />
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
  import Experience from './Hud/Experience'
  import Gold from './Hud/Gold'
  import Health from './Hud/Health'
  import Mana from './Hud/Mana'
  import Menu from './Hud/Menu'
  import Spells from './Hud/Spells'

  export default {
    name: 'Hud',
    components: {
      Experience,
      Gold,
      Health,
      Mana,
      Menu,
      Spells
    }
  }
</script>

<style lang="scss" scoped>
  #hud {
    height: 15vh;

    & .column {
      display: flex;
      align-items: center;
    }

    &.footer {
      padding: 0;
    }
  }
</style>