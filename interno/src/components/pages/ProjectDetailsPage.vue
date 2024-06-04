<template>
  <div class="project__details">
    <HeaderComponent />
    <BaseBanner :image="`url(${image})`"></BaseBanner>
    <ProjectDetailsContent />
    <ProjectDetailsSlider />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "../HeaderComponent.vue";
import BaseBanner from "../BaseBanner.vue";
import ProjectDetailsContent from "../ProjectDetailsContent.vue";
import ProjectDetailsSlider from "../ProjectDetailsSlider.vue";
import FooterComponent from "../FooterComponent.vue";

export default {
  neme: "ProjectDetailsPage",
  components: {
    HeaderComponent,
    BaseBanner,
    ProjectDetailsContent,
    ProjectDetailsSlider,
    FooterComponent,
  },
  data() {
    return {
      image: "ProjectDetailsBanner.png",
    };
  },
};
</script>

<style lang="scss"></style>
