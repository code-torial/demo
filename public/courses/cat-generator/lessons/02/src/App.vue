<script>
import { ref } from 'vue'

export default {
  setup() {
    const imgUrl = ref("")
    return {
      imgUrl,
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
