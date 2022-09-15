<template>
  <section id="about" class="about section">
    <h1 class="section__title">About</h1>
    <p class="section__subtitle">My Introduction</p>
    <div class="row">
      <div class="col-md-6">
        <div class="img">
          <img src="/___a.jpeg" alt="" />
        </div>
      </div>
      <div class="col-md-6">
        <div class="content">
          <p>
            Fullstack Developer and an inspirational mentor with over 4
            years of experience in software development. Recognized for
            demonstrating strong analytical skills and proven software
            development skills. Expert in <code>console.log("JavaScript");<br> </code> <code>echo "PHP";</code> and <br>
            <code>print("Python")</code>. <br>
            Resourceful and well-organized with excellent leadership and
            team-building record. Creative in solving problems and always
            coming up with innovative ideas. Excellent in working as part
            of a team or individually. Effective and articulate
            communicator with all levels of employees and perfect with
            googling.
          </p>
          <div class="stats">
            <div class="stat">
              <h3>{{experience}}+</h3>
              <p>Years Experience</p>
            </div>
            <div class="stat">
              <h3>08+</h3>
              <p>Completed Projects</p>
            </div>
            <div class="stat">
              <h3>{{compCount}}+</h3>
              <p>Companies Worked</p>
            </div>
          </div>
          <a href="pdf/resume.pdf" target="_blank" class="btn btn_primary mt-5">
            Download CV <i class="uil uil-import mx-2"></i>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref } from 'vue';
import data from '../config/data';

export default {
  name: 'AboutSection',
  setup() {
    const compCount = data.companies.length
    const experience = ref(Number(new Date().getFullYear()) - 2018)
    return {
      experience,
      compCount
    }
  }
}
</script>