<script setup>
import { ref, computed } from 'vue'

const props = defineProps(['height', 'border', 'vid', 'width'])

const url = computed(() => {
  return "https://www.youtube.com/embed/" + props.vid
})

const border = ref(props.border || 0)
const height = ref(props.height || 315)
const width = ref(props.width || 560)
</script>

<template>
  <div>
    <iframe :width="width" :height="height" :src="url" title="YouTube video player" :frameborder="border"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
  </div>
</template>
