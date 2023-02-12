<template>
  <section id="section-about">
    <div class="container relative">
      <div class="row">
        <div class="col-md-12 text-center wow fadeInUp">
          <h2 v-if="title">{{ title }}</h2>
          <div class="space-border"></div>
        </div>
        <div v-if="text" class="col-md-8 offset-md-2 text-center wow fadeInUp">
          <p>{{ text }}</p>
        </div>
        <div class="spacer-single"></div>
        <skill-item
          v-for="(item, index) in skills" :key="index"
          :percent="item.percent"
          :name="item.name"
        />
      </div>
    </div>
  </section>
</template>

<script>
import SkillItem from "~/components/elements/about/SkillItem";
export default {
  name: "SectionAbout",
  components: { SkillItem },
  props: {
    title: {
      type: String,
      default: ''
    },
    text: {
      type: String,
      default: ''
    },
    skills: {
      type: Array,
      default: ()=>{}
    }
  },
}
</script>

<style scoped>

</style>
