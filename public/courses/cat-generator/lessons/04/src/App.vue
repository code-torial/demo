<script>
import { ref } from 'vue'

function getImageUrl() {
  const url = new URL('https://cataas.com/cat')
  url.searchParams.set('width', 300)
  url.searchParams.set('height', 300)
  return url.toString()
}

export default {
  setup() {
    const imgUrl = ref(getImageUrl())
    function newImage() {
      imgUrl.value = getImageUrl()
    }
    return {
      imgUrl,
      newImage
    }
  },
}
</script>

<template>
  <div class="content">
    <h1>Here's your cat</h1>
    <img :src="imgUrl" />
    <button>Moar plz</button>
  </div>
</template>

<style>
.content {
  margin: 20px auto;
  display: flex;
  flex-direction: column;
  max-width: 300px;
  justify-content: center;
  align-items: center;
  gap: 15px;
}

.content h1 {
  margin: 0;
}
</style>
