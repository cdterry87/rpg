<template>
  <div>
    <Game />
    <Hud />
  </div>
</template>

<script>
import Game from './components/Game'
import Hud from './components/Hud'

export default {
  name: 'App',
  components: {
    Game,
    Hud
  }
}
</script>

<style lang="scss">

</style>
