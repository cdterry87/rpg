<template>
  <div id="spells" class="buttons">
    <button class="button is-danger is-outlined">
      <span class="icon">
        <i class="fas fa-fire-alt"></i>
      </span>
    </button>

    <button class="button is-info is-outlined">
      <span class="icon">
        <i class="fas fa-snowflake"></i>
      </span>
    </button>

    <button class="button is-warning is-outlined">
      <span class="icon">
        <i class="fas fa-bolt"></i>
      </span>
    </button>

    <button class="button is-success is-outlined">
      <span class="icon">
        <i class="fas fa-wind"></i>
      </span>
    </button>
  </div>
</template>

<script>
  export default {
    name: 'Spells'
  }
</script>

<style lang="scss" scoped>
  #spells {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
  }
</style>