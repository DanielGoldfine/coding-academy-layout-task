<template>
  <main class="features-list">
    <section class="features-grid-container">
      <featurePreview
        v-for="(feature, idx) in features"
        :key="idx"
        :imgUrl="feature.imgUrl"
        :title="feature.title"
        :txt="feature.txt"
      />
    </section>
  </main>
</template>

<script>
import featurePreview from "./feature-preview.vue";

export default {
  name: "features-list",
  data() {
    return {
      features: [
        {
          imgUrl: require("../assets/icon-access-anywhere.svg"),
          title: "Access your files, anywhere",
          txt:
            "The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere."
        },
        {
          imgUrl: require("../assets/icon-security.svg"),
          title: "Security you can trust",
          txt:
            "2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files."
        },
        {
          imgUrl: require("../assets/icon-collaboration.svg"),
          title: "Real-time collaboration",
          txt:
            "Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required."
        },
        {
          imgUrl: require("../assets/icon-any-file.svg"),
          title: "Store any type of file",
          txt:
            "Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared."
        }
      ]
    };
  },
  components: {
    featurePreview
  }
};
</script>