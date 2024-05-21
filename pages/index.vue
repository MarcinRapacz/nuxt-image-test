<template>
  <nav :class="$style.root">
    <NuxtLink to="/without-nuxt-image">Without nuxt image</NuxtLink>
    <NuxtLink to="/base-nuxt-image">Base nuxt image</NuxtLink>
    <NuxtLink to="/with-webp">With webp</NuxtLink>
    <NuxtLink to="/with-width-height">With weidth height</NuxtLink>
    <NuxtLink to="/with-sizes">With sizes</NuxtLink>
    <NuxtLink to="/with-lazy">With lazy</NuxtLink>
    <NuxtLink to="/with-placeholder">With placeholder</NuxtLink>
  </nav>
</template>

<style lang="scss" module>
.root {
  margin: 2rem;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
</style>
