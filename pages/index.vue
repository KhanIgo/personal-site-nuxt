<template>
  <IndexHero
    userName="I Am Khan Igor"
    :job="['Developer', 'Frontend', 'Fullstack', 'Freelancer']"
    :locations="[{
      loc1: 'Russia',
      loc2: 'Khabarovsk',
    }]"
  />
</template>

<script>
import IndexHero from "~/components/sections/IndexHero";
export default {
  name: 'IndexPage',
  components: { IndexHero },
  layout: 'main',

  head() {
    return {
      script: [
        { src: "/js/recaptcha.js" },
        { src: "/js/typed.js" }
      ]
    };
  }
}
</script>

<style lang="scss">
:root {
  --primary-color: #CF1F1F;
  --primary-color-rgb: 207, 31, 31;
}
</style>
