<template>
  <nav class="flex justify-end px-10">
    <ul class="flex gap-2 max-w-lg text-center">
      <li class="max-w-20 h-16">
        <NuxtLink to="/" class="nav-link" data-label="Home" exact>
          <span> Home </span>
        </NuxtLink>
      </li>
      <li class="max-w-20 h-16">
        <NuxtLink to="/about" class="nav-link" data-label="About">
          <span> About </span>
        </NuxtLink>
      </li>
      <li class="max-w-20 h-16">
        <NuxtLink to="/projects" class="nav-link" data-label="Projects">
          <span class="z-10"> Projects </span>
        </NuxtLink>
      </li>
      <li class="max-w-20 h-16">
        <NuxtLink to="/contact" class="nav-link" data-label="Contact">
          <span> Contact </span>
        </NuxtLink>
      </li>
      <li class="max-w-20 h-16">
        <NuxtLink to="/blog" class="nav-link" data-label="Blog">
          <span> Blog </span>
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="postcss" scoped>
.nuxt-link-active {
  @apply bg-secondary rounded-b-full;
}

.nav-link {
  @apply relative h-full w-20 inline-block px-3 py-6 text-black dark:text-white rounded-b-full;
  &::after {
    content: '';
    transition: all 0.3s;
    @apply absolute top-0 left-0 w-full h-0 px-3 py-1 rounded-b-full bg-secondary;
  }
  &:not(.nuxt-link-active):hover::after {
    content: attr(data-label);
    @apply h-full py-6 z-0;
  }
}
</style>
