<template>
  <section id="skills" class="skills section">
    <h1 class="section__title">Brands</h1>
    <p class="section__subtitle">Brands I have worked with</p>
    <div class="row">
      <div v-for="item in brandsData" :key="item.id" class="col-md-3 brand_logo_wrapper">
        <div class="brand_logo_wrapper mb-5">
          <img class="brand_logo my-auto" :src="item.logo" :alt="item.name">
          <i class="uil uil-external-link-alt mx-3"></i>
        </div>
      </div>
      <div class="col-md-3 brand_logo_wrapper">
        <div class="brand_logo_wrapper">
          <svg class="brand_logo ammiel" width="48" height="48" fill="none" xmlns="http://www.w3.org/2000/svg">
            <mask id="a" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="48" height="48">
              <path fill="#D9D9D9" d="M0 0h48v48H0z"></path>
            </mask>
            <g mask="url(#a)">
              <path
                d="M31.945 12.293c2.332-1.585 5.527-.324 6.15 2.425l4.56 20.15c.71 3.135-2.38 5.784-5.37 4.605l-21.65-8.541c-2.99-1.18-3.438-5.224-.78-7.03l17.09-11.61Z"
                fill="#9174DC"></path>
              <path
                d="M15.194 12.293c-2.331-1.585-5.526-.324-6.149 2.425l-4.56 20.15c-.71 3.135 2.38 5.784 5.369 4.605l21.65-8.541c2.99-1.18 3.439-5.224.78-7.03l-17.09-11.61Z"
                fill="#6036D0"></path>
              <path
                d="M20.339 7.593c1.585-2.354 5.05-2.354 6.635 0l11.688 17.352c1.79 2.657-.114 6.235-3.318 6.235H11.97c-3.204 0-5.108-3.578-3.318-6.235L20.339 7.593Z"
                fill="#734DD5"></path>
            </g>
          </svg>
          <i class="uil uil-external-link-alt"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref } from 'vue';
import data from '../config/data';

export default {
  name: 'BrandSection',
  setup() {
    const brandsData = ref(data.companies);
    return {
      brandsData
    }
  }
}
</script>
