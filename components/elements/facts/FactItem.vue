<template>
  <div class="col-md-3 wow fadeIn" :data-wow-delay="delay">
    <div class="de_count text-center">
      <h3 class="timer" :data-to="value" data-speed="2500">0</h3>
      <span>{{ name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "FactItem",
  props: {
    name: {
      type: String,
      default: ''
    },
    value: {
      type: String,
      default: ''
    },
  },
  computed: {
    delay() {
      return (this.$vnode.key*0.25)+'s';
    }
  }
}
</script>

<style scoped>

</style>
