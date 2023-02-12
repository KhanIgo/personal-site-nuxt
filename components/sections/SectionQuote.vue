<template>
  <section id="section-my-quote" aria-label="section" class="jarallax no-top no-bottom">
    <div class="de-gradient-edge-top"></div>
    <img src="/images/background/2.jpg" class="jarallax-img" alt="">
    <div class="v-center">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-10 offset-md-1">
            <blockquote class="q-big wow fadeIn" data-wow-duration="3s">
              <i class="d-big icon_quotations"></i>
              <span v-if="text">{{ text }}</span>
              <span v-if="author" class="d-quote-by">{{  author }}</span>
            </blockquote>
            <div class="spacer-double"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="de-gradient-edge-bottom"></div>
  </section>
</template>

<script>
export default {
  name: "SectionQuote",
  props: {
    text: {
      type: String,
      default: ''
    },
    author: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>

</style>
