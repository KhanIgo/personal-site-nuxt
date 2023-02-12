<template>
  <section id="section-about">
    <div class="container relative">
      <div class="row">
        <div class="col-md-12 text-center wow fadeInUp">
          <h2 v-if="title">{{ title }}</h2>
          <div class="space-border"></div>
        </div>
        <div v-if="text" class="col-md-8 offset-md-2 text-center wow fadeInUp">
          <p>{{ text }}</p>
        </div>
        <div class="spacer-single"></div>
        <div
          v-for="(item, index) in skills" :key="index"
          class="col-lg-3 position-relative wow fadeIn"
          :data-wow-delay="((index+1)*0.2)+'s'">
          <div class="position-relative">
            <div class="progressbar" data-animate="false">
              <div class="circle" :data-percent="item.percent">
                <div></div>
              </div>
              <h4>{{ item.name }}</h4>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "IndexAbout",
  props: {
    title: {
      type: String,
      default: ''
    },
    text: {
      type: String,
      default: ''
    },
    skills: {
      type: Array,
      default: ()=>{}
    }
  },
}
</script>

<style scoped>

</style>
