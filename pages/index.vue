<template>
  <div class="flex justify-between">
    <PortfolioWord />
    <nuxt-img
      provider="cloudinary"
      src="/v1621173616/me_u2wdim.png"
      width="500"
      height="500"
      fit="fill"
      :modifiers="{ gravity: 'subject' }"
    />
    <div>s</div>
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

<style lang="postcss" scoped></style>
