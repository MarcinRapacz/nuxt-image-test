<script setup lang="ts">
import { getMedia } from "~/utils/getLinks";

const media = getMedia();
</script>

<template>
  <div :class="$style.root">
    <div :class="$style.container" v-for="it in media">
      <NuxtImg
        :src="it.src"
        :alt="it.src"
        :key="it.src"
        :width="it.width"
        :height="it.height"
        format="webp"
      />
    </div>
  </div>
</template>

<style lang="scss" module>
.root {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  max-width: 1200px;
  margin: 0 auto;
  column-gap: 1rem;
  row-gap: 3rem;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}

.container {
  width: 100%;
  height: 400px;
}
</style>
