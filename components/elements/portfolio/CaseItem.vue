<template>
  <div class="col-md-4 item">
    <div class="de_modal wow" :data-url="url">
      <div class="card-image-1 mod-c" data-tilt>
        <div class="d-text">
          <h3>{{ name }}</h3>
          <h5 class="d-tag">{{ tag }}</h5>
        </div>
        <img :src="img" class="img-fluid" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CaseItem",
  props: {
    url: {
      type: String,
      default: ''
    },
    name: {
      type: String,
      default: ''
    },
    tag: {
      type: String,
      default: ''
    },
    img: {
      type: String,
      default: ''
    },

  }
}
</script>

<style scoped>

</style>
