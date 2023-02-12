<template>
  <div class="col-lg-6 wow fadeInUp">
    <div class="p-4">
      <h3 class="s_border">{{ title }}</h3>
      <ul class="d_timeline">
        <resume-item
          v-for="(item, index) in items" :key="index"
          :date="item.date"
          :text="item.text"
        />
      </ul>
    </div>
  </div>
</template>

<script>
import ResumeItem from "~/components/elements/resume/ResumeItem";
export default {
  name: "ResumeColumn",
  components: { ResumeItem },
  props: {
    title: {
      type: String,
      default: ''
    },
    items: {
      type: Array,
      default: ()=>{}
    },
  }
}
</script>

<style scoped>

</style>
