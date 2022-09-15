<template>
  <div class="container">
    <div class="alert alert-warning" role="alert">
      Site is still under development! <i class="uil uil-warning"></i>
    </div>
    <Navbar />
    <main class="main">
      <HeroSection />
      <AboutSection />
      <SkillsSection />
      <ContactSection />
    </main>
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import HeroSection from "../components/HeroSection.vue";
import AboutSection from "../components/AboutSection.vue";
import SkillsSection from "../components/SkillsSection.vue";
import ContactSection from "../components/ContactSection.vue";
export default {
  name: "HomePage",
  components: { Navbar, HeroSection, AboutSection, SkillsSection, ContactSection }
}
</script>