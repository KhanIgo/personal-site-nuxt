<template>
  <li class="d_timeline-item">
    <h3 class="d_timeline-title">{{ date }}</h3>
    <p class="d_timeline-text" v-html="text"></p>
  </li>
</template>

<script>
export default {
  name: "ResumeItem",
  props: {
    date: {
      type: String,
      default: ''
    },
    text: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>

</style>
