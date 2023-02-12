<template>
  <div id="carousel-blog" class="owl-carousel wow fadeInUp">
    <blog-post
      v-for="(item, index) in posts" :key="index"
      :url="item.url"
      :image="item.image"
      :title="item.title"
      :text="item.text"
    />
  </div>
</template>

<script>
import BlogPost from "~/components/elements/blog/BlogPost";
export default {
  name: "BlogCarousel",
  components: { BlogPost },
  props: {
    posts: {
      type: Array,
      default: ()=>{}
    }
  }
}
</script>

<style scoped>

</style>
