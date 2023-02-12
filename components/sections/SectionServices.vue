<template>
  <section id="section-services" class="no-bottom">
    <div class="container relative">
      <div class="row">
        <div v-if="title" class="col-md-12 text-center wow fadeInUp">
          <h2>{{ title }}</h2>
          <div class="space-border"></div>
        </div>
        <div class="spacer-single"></div>
        <div class="row g-0">
          <service-item
            v-for="(item, index) in services" :key="index"
            :icon="item.icon"
            :name="item.name"
            :text="item.text"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ServiceItem from "~/components/elements/services/ServiceItem";
export default {
  name: "SectionServices",
  components: { ServiceItem },
  props: {
    title: {
      type: String,
      default: ''
    },
    services: {
      type: Array,
      default: ()=>{}
    }
  }
}
</script>

<style scoped>

</style>
