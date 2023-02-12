<template>
  <div
    class="col-lg-4 wow fadeIn"
    :data-wow-delay="delay">
    <div class="de_3d-box">
      <div class="d-inner">
        <i class="icon_genius id-color"
           :class="icon"
        ></i>
        <div class="text">
          <h3>{{ name }}</h3>
          {{ text }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ServiceItem",
  props: {
    icon: {
      type: String,
      default: ''
    },
    name: {
      type: String,
      default: ''
    },
    text: {
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
