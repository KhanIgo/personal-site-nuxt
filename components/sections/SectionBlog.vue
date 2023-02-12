<template>
  <section id="section-blog" class="no-bottom">
    <div class="container relative">
      <div class="row">
        <div v-if="title" class="col-md-12 text-center wow fadeInUp">
          <h2>{{ title }}</h2>
          <div class="space-border"></div>
        </div>
      </div>
      <blog-carousel
        :posts="posts"
      />
    </div>
  </section>
</template>

<script>
import BlogCarousel from "~/components/elements/blog/BlogCarousel";
export default {
  name: "SectionBlog",
  components: { BlogCarousel },
  props: {
    title: {
      type: String,
      default: ''
    },
    posts: {
      type: Array,
      default: ()=>{}
    }
  }
}
</script>

<style scoped>

</style>
