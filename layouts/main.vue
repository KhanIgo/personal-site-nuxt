<template>
  <div id="wrapper">
    <!-- header begin -->
    <header class="transparent">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="de-flex sm-pt10">
              <div class="de-flex-col">
                <div class="de-flex-col">
                  <!-- logo begin -->
                  <div id="logo">
                    <a href="index.html">
                      <img alt="" class="logo" src="images/logo.png" />
                      <img alt="" class="logo-2" src="images/logo.png" />
                    </a>
                  </div>
                  <!-- logo close -->
                </div>
              </div>
              <div class="de-flex-col header-col-right">
                <ul id="mainmenu">
                  <li><a class="active" href="#top">Home<span></span></a></li>
                  <li><a href="#section-about">About me<span></span></a></li>
                  <li><a href="#section-services">What I Do<span></span></a></li>
                  <li><a href="#section-portfolio">Portfolio<span></span></a></li>
                  <li><a href="#section-resume">My Resume<span></span></a></li>
                  <li><a href="#section-blog">Blog<span></span></a></li>
                  <li><a href="#section-contact">Contact Me<span></span></a></li>
                </ul>
                <div class="menu_side_area">
                  <span id="menu-btn"></span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
    <!-- header close -->
    <!-- content begin -->
    <div id="content" class="no-bottom no-top">
      <div id="top"></div>

      <!-- page preloader begin -->
      <div id="preloader">
        <div class="preloader1"></div>
      </div>
      <!-- page preloader close -->

      <!-- float text begin -->
      <div class="float-text">
        <div class="de_social-icons">
          <a href="#"><i class="fa fa-facebook fa-lg"></i></a>
          <a href="#"><i class="fa fa-twitter fa-lg"></i></a>
          <a href="#"><i class="fa fa-instagram fa-lg"></i></a>
        </div>
        <span>Follow Me</span>
      </div>
      <!-- float text close -->
      <nuxt />
    </div>
    <!-- content close -->
    <a id="back-to-top" href="#"></a>
    <!-- footer begin -->
    <footer>
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <a href="index.html">
              <span class="copy">&copy; Copyright 2022 - Kyros by Designesia</span>
            </a>
          </div>
          <div class="col-md-6">
            <div class="social-icons">
              <a href="#"><i class="fa fa-facebook fa-lg"></i></a>
              <a href="#"><i class="fa fa-twitter fa-lg"></i></a>
              <a href="#"><i class="fa fa-linkedin fa-lg"></i></a>
              <a href="#"><i class="fa fa-pinterest fa-lg"></i></a>
              <a href="#"><i class="fa fa-rss fa-lg"></i></a>
            </div>
          </div>
        </div>
      </div>
    </footer>
    <!-- footer close -->
  </div>
</template>

<script>
export default {
    head() {
      return {
        link: [
          {rel: 'stylesheet', href: '/css/bootstrap.min.css'},
          {rel: 'stylesheet', href: '/css/plugins.css'},
          {rel: 'stylesheet', href: '/css/style.css'},
          {rel: 'stylesheet', href: '/css/coloring.css'},
        ],
        script: [
          { src: '/js/plugins.js', type: 'text/javascript' },
          { src: "/js/designesia.js" },
          { src: "https://www.google.com/recaptcha/api.js", async: true, defer: true },
          { src: "/js/form.js" },
        ],
      }
    }
}
</script>
