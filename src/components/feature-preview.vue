<template>
  <main class="feature-preview flex column align-center justify-space-between">
    <img :src="imgUrl" alt />
    <div class="text flex column align-center">
      <h5>{{title}}</h5>
      <p>{{txt}}</p>
    </div>
  </main>
</template>

<script>
export default {
  name: "feature-preview",
  props: ["imgUrl", "title", "txt"]
};
</script>