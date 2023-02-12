<template>
  <section id="section-portfolio" class="no-bottom">
    <div class="container relative">
      <div class="row">
        <div v-if="title" class="col-md-12 text-center wow fadeInUp">
          <h2>{{ title }}</h2>
          <div class="space-border"></div>
        </div>
      </div>
      <div id="gallery" class="row sequence">
        <case-item v-for="(item, index) in cases" :key="index"
           :url="item.url" :name="item.name" :tag="item.tag" :img="item.img"
        />
      </div>
    </div>
  </section>
</template>

<script>
import CaseItem from "~/components/elements/portfolio/CaseItem";
export default {
  name: "SectionPortfolio",
  components: {
    CaseItem
  },
  props: {
    title: {
      type: String,
      default: ''
    },
    cases: {
      type: Array,
      default: ()=>{}
    }
  },
}
</script>

<style scoped>

</style>
