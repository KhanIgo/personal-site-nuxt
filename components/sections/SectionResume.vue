<template>
  <section id="section-resume">
    <div class="container relative">
      <div class="row">
        <div v-if="title" class="col-md-12 text-center wow fadeInUp">
          <h2>{{ title }}</h2>
          <div class="space-border"></div>
        </div>
      </div>
      <div class="row gh-5">
        <resume-column
          :title="titleCol1"
          :items="itemsCol1"
        />
        <resume-column
          :title="titleCol2"
          :items="itemsCol2"
        />
      </div>
    </div>
  </section>
</template>

<script>
import ResumeColumn from "~/components/elements/resume/ResumeColumn";
export default {
  name: "SectionResume",
  components: { ResumeColumn },
  props: {
    title: {
      type: String,
      default: ''
    },
    titleCol1: {
      type: String,
      default: ''
    },
    titleCol2: {
      type: String,
      default: ''
    },
    itemsCol1: {
      type: Array,
      default: ()=>{}
    },
    itemsCol2: {
      type: Array,
      default: ()=>{}
    }
  }

}
</script>

<style scoped>

</style>
