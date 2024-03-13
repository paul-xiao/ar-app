<script setup lang="ts">
import '@ar-js-org/ar.js'
</script>

<template>
  <a-scene embedded arjs>
    <a-marker preset="hiro">
      <!-- we use cors proxy to avoid cross-origin problems ATTENTION! you need to set up your server -->
      <a-entity position="0 0 0" scale="0.05 0.05 0.05" gltf-model="./src/assets/scene.gltf"></a-entity>
    </a-marker>
    <a-entity camera></a-entity>
  </a-scene>
</template>
