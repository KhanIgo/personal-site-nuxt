<template>
  <div id="wrapper">
    <site-header />
    <!-- content begin -->
    <div id="content" class="no-bottom no-top">
      <div id="top"></div>
      <modal />
      <preloader />
      <float-text />
      <nuxt />
    </div>
    <!-- content close -->

    <btn-to-top />
    <site-footer />
  </div>
</template>

<script>
import SiteHeader from "~/components/header/SiteHeader";
import SiteFooter from "~/components/footer/SiteFooter";
import BtnToTop from "~/components/elements/BtnToTop";
import Preloader from "~/components/elements/Preloader";
import FloatText from "~/components/elements/FloatText";
import Modal from "~/components/ui/Modal";
export default {
  components: { SiteHeader, SiteFooter, Preloader, BtnToTop, FloatText, Modal },
    head() {
      return {
        link: [
          {rel: 'stylesheet', href: '/css/bootstrap.min.css'},
          {rel: 'stylesheet', href: '/css/plugins.css'},
          {rel: 'stylesheet', href: '/css/style.css'},
          {rel: 'stylesheet', href: '/css/coloring.css'},
        ],
        script: [
          { src: '/js/plugins.js'},
          { src: "/js/designesia.js" },
          { src: "https://www.google.com/recaptcha/api.js", async: true, defer: true },
          { src: "/js/form.js" },
        ],
        bodyAttrs: {
          class: 'onepage dark-scheme'
        }
      }
    }
}
</script>
