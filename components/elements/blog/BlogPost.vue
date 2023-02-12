<template>
  <div class="bloglist item">
    <div class="post-content">
      <div class="post-image">
        <div class="de_modal" :data-url="url"><img alt="" :src="image" class="lazy grayscale"></div>
      </div>
      <div class="post-text">
        <h4 class="de_modal" :data-url="url">{{ title }}</h4>
        <p>{{ text }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BlogPost",
  props: {
    url: { type: String, default: '' },
    image: { type: String, default: '' },
    title: { type: String, default: '' },
    text: { type: String, default: '' },
  }
}
</script>

<style scoped>

</style>
