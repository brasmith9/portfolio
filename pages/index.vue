<template>
  <Home />
</template>

<script lang="js">
import { onMounted } from 'vue';
import Home from './Home.vue';
export default {
  name: "IndexPage",
  components: { Home },
  setup() {
    onMounted(()=> {
      document.body.classList.add(['_dark']);
    });

  }
}
</script>
