<template>
  <main class="team-list-container">
    <section class="team-list flex align-center justify-space-between">
      <teamMemberPreview
        v-for="(member, idx) in members"
        :key="idx"
        :avatar="member.avatar"
        :desc="member.desc"
        :name="member.name"
        :position="member.position"
      />
    </section>
    <img class="quotes-img" src="../assets/bg-quotes.png" alt="">
  </main>
</template>

<script>
import teamMemberPreview from "./team-member-preview.vue";

export default {
  name: "team-list",
  data() {
    return {
      members: [
        {
          avatar: require("../assets/profile-1.jpg"),
          desc:
            "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
          name: "Satish Patel",
          position: "Founder & CEO, Huddle"
        },
        {
          avatar: require("../assets/profile-2.jpg"),
          desc:
            "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
          name: "Bruce McKenzie",
          position: "Founder & CEO, Huddle"
        },
        {
          avatar: require("../assets/profile-3.jpg"),
          desc:
            "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
          name: "Iva Boyd",
          position: "Founder & CEO, Huddle"
        }
      ]
    };
  },
  components: {
    teamMemberPreview
  }
};
</script>