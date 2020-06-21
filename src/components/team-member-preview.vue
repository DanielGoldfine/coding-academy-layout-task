<template>
  <main class="team-member-preview flex column align-end justify-space-between">
    <h5>{{desc}}</h5>
    <div class="avatar flex align-center">
      <div class="img-container">
        <img :src="avatar" alt />
      </div>
      <div class="text flex column justify-space-between">
        <h6>{{name}}</h6>
        <p>{{position}}</p>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "member-preview",
  props: ["avatar", "desc", "name", "position"]
};
</script>