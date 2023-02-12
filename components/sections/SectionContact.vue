<template>
  <section id="section-contact" class="jarallax">
    <div class="de-gradient-edge-top"></div>
    <img :src="bgImage" class="jarallax-img" alt="">
    <div class="container z-index-1000">
      <div class="row">
        <div v-if="title" class="col-md-12 text-center wow fadeInUp">
          <h2>{{ title }}</h2>
          <div class="space-border"></div>
        </div>
        <div class="col-lg-8 offset-lg-2 wow fadeInUp">
          <div class="contact_form_wrapper">
            <contact-form />
          </div>
          <div class="spacer-double"></div>
          <div class="row text-center wow fadeInUp">
            <contact-item
              v-for="(item, index) in items" :key="index"
              :title="item.title"
              :text="item.text"
            />
          </div>
        </div>
      </div>
    </div>
    <div class="de-gradient-edge-bottom"></div>
  </section>
</template>

<script>
import ContactForm from "~/components/forms/ContactForm";
import ContactItem from "~/components/elements/contacts/ContactItem";
export default {
  name: "SectionContact",
  components: { ContactForm, ContactItem },
  props: {
    title: { type: String, default: '' },
    bgImage: { type: String, default: '' },
    items: { type: Array, default: ()=>{} },
  }
}
</script>

<style scoped>

</style>
