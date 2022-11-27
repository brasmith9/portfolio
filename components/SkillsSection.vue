<template>
  <section id="skills" class="skills section">
    <h1 class="section__title">Skills</h1>
    <p class="section__subtitle">My Stack</p>
    <div class="row inner_skills">
      <div v-for="item in skillData" :key="item.id" class="col-md-6">
        <div class="skill">
          <div
            class="skill__head collapsed border-bottom"
            data-bs-toggle="collapse"
            :href=item.id
            role="button"
            aria-expanded="false"
            aria-controls="frontend"
          >
            <h5 class="d-flex align-items-center">
              <i class="uil uil-brackets-curly"></i>
              {{item.stack}}
            </h5>
            <i class="uil uil-angle-down"></i>
          </div>
          <div :id=item.id class="collapse multi-collapse show">
            <div class="card card-body">
              <div v-for="skill in item.skill" :key="skill.id" class="skill__progress">
                <div class="skill__title">
                  <p>{{skill.tool}}</p>
                  <p>{{skill.percentage}}</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="50"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref } from 'vue';
import data from '../config/data';

  export default {
    name: 'SkillsSection',
    setup() {
      const skillData = ref(data.skills);
      return {
        skillData
      }
    }
  }
</script>
