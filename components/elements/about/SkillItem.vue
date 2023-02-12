<template>
  <div
    class="col-lg-3 position-relative wow fadeIn"
    :data-wow-delay="delay">
    <div class="position-relative">
      <div class="progressbar" data-animate="false">
        <div class="circle" :data-percent="percent">
          <div></div>
        </div>
        <h4>{{ name }}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SkillItem",
  props: {
    name: {
      type: String,
      default: ''
    },
    percent: {
      type: String,
      default: ''
    },
  },
  computed: {
    delay() {
      return ((this.$vnode.key+1)*0.2)+'s';
    }
  }
}
</script>

<style scoped>

</style>
