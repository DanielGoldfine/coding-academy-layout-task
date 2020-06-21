<template>
  <main class="home-page-container main-container flex column align-center">
    <navBar />
    <heroSection />
    <featuresList />
    <middleSection />
    <teamList />
  </main>
</template>

<script>
import navBar from "../components/nav-bar.vue";
import heroSection from "../components/hero-section.vue";
import featuresList from "../components/features-list.vue";
import middleSection from "../components/middle-section.vue";
import teamList from "../components/team-list.vue";

export default {
  name: "home-page",
  components: {
    navBar,
    heroSection,
    featuresList,
    middleSection,
    teamList
  }
};
</script>