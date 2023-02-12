<template>
  <section id="section-fun-facts" aria-label="section" class="jarallax">
    <div class="de-gradient-edge-top"></div>
    <img src="images/background/3.jpg" class="jarallax-img" alt="">
    <div class="container">
      <div class="row">
        <fact-item
          v-for="(item, index) in items" :key="index"
          :name="item.name"
          :value="item.value"
        />
      </div>
    </div>
    <div class="de-gradient-edge-bottom"></div>
  </section>
</template>

<script>
import FactItem from "~/components/elements/facts/FactItem";
export default {
  name: "SectionFacts",
  components: { FactItem },
  props: {
    items: {
      type: Array,
      default: ()=>{}
    }
  }
}
</script>

<style scoped>

</style>
