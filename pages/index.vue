<template>
  <div>
    <index-hero
      user-name="I Am Khan Igor"
      :job="['Developer', 'Frontend', 'Fullstack', 'Freelancer']"
      :locations="[{
        loc1: 'Russia',
        loc2: 'Khabarovsk',
      }]"
    />
    <index-about
      title="About Me"
      text="I am a website designer from Lousiana, with a strong focus in UI/UX design. I love to get new experiences and always learn from my surroundings. I've done more than 285 projects. You can check it through portfolio section on
            this website. I looking forward to any opportunities and challenges."
      :skills="[
        { name: 'HTML', percent: 90 },
        { name: 'CSS', percent: 85 },
        { name: 'PHP', percent: 80 },
        { name: 'jQuery', percent: 75 }
      ]"
    />
  </div>
</template>

<script>
import IndexHero from "~/components/sections/IndexHero";
import IndexAbout from "~/components/sections/IndexAbout";
export default {
  name: 'IndexPage',
  components: { IndexHero, IndexAbout },
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
