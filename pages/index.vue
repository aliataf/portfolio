<template>
  <div class="container">
    <PortfolioWord />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import PortfolioWord from '@/components/PortfolioWord.vue'

export default Vue.extend({
  components: {
    PortfolioWord,
  },
})
</script>

<style lang="postcss" scoped>
.container {
  @apply min-h-screen w-screen mx-auto;
}
</style>
