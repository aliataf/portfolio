<template>
  <div
    class="
      portfolio-word-container
      flex flex-col
      justify-around
      items-center
      max-w-max
      p-4
    "
  >
    <div class="not-o">P</div>
    <div class="o">O</div>
    <div class="not-o">RTF</div>
    <div class="o">O</div>
    <div class="not-o">LI</div>
    <div class="o">O</div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="postcss" scoped>
.portfolio-word-container {
  height: calc(100vh - theme(height.16));
}

.not-o {
  font-size: 50px;
  @apply text-black dark:text-white font-extrabold;
}

.o {
  font-size: 80px;
  @apply text-secondary;
}
</style>
