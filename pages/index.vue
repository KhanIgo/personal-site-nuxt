<template>
  <div>
    <section-index-hero
      user-name="I Am Khan Igor"
      :job="['Developer', 'Frontend', 'Fullstack', 'Freelancer']"
      :locations="[{
        loc1: 'Russia',
        loc2: 'Khabarovsk',
      }]"
    />
    <section-about
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
    <section-quote
      text="Do more than is required. What is the distance between someone who achieves their goals consistently and those who spend their lives and careers merely following? The extra mile."
      author="Khan Igor"
    />
    <section-services />
    <section-portfolio />
    <section-resume />
    <section-facts />
    <section-blog />
    <section-contact />
  </div>
</template>

<script>
import SectionIndexHero from "~/components/sections/SectionIndexHero";
import SectionAbout from "~/components/sections/SectionAbout";
import SectionQuote from "~/components/sections/SectionQuote";
import SectionServices from "~/components/sections/SectionServices";
import sectionPortfolio from "~/components/sections/SectionPortfolio";
import SectionResume from "~/components/sections/SectionResume";
import SectionFacts from "~/components/sections/SectionFacts";
import SectionBlog from "~/components/sections/SectionBlog";
import SectionContact from "~/components/sections/SectionContact";
export default {
  name: 'IndexPage',
  components: {
    SectionIndexHero, SectionAbout, SectionQuote,
    SectionServices, sectionPortfolio, SectionResume,
    SectionFacts, SectionBlog, SectionContact
  },
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
