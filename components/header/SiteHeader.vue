<template>
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
                    <img alt="" class="logo" src="/images/logo.png" />
                    <img alt="" class="logo-2" src="/images/logo.png" />
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
</template>

<script>
export default {
  name: 'SiteHeader'
}
</script>

<style scoped>

</style>
