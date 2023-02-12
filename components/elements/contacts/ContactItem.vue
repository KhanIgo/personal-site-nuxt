<template>
  <div class="col-md-4">
    <div class="wm-1"></div>
    <h6>{{ title }}</h6>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: "ContactItem",
  props: {
    title: { type: String, default: '' },
    text: { type: String, default: '' },
  }
}
</script>

<style scoped>

</style>
