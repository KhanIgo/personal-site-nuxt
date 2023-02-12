<template>
  <form name="contactForm" id="contact_form" class="form-border" method="post" action="#">
    <div class="row">
      <div class="col-md-4">
        <div class="field-set">
          <input type="text" name="Name" id="name" class="form-control" placeholder="Your Name" required>
        </div>
      </div>
      <div class="col-md-4">
        <div class="field-set">
          <input type="text" name="Email" id="email" class="form-control" placeholder="Your Email" required>
        </div>
      </div>
      <div class="col-md-4">
        <div class="field-set">
          <input type="text" name="phone" id="phone" class="form-control" placeholder="Your Phone" required>
        </div>
      </div>
    </div>
    <div class="text-center">
      <div class="field-set">
        <textarea name="message" id="message" class="form-control" placeholder="Your Message" required></textarea>
      </div>
      <div class="g-recaptcha" data-sitekey="copy-your-site-key-here"></div>
      <div id='submit' class="mt10">
        <input type='submit' id='send_message' value='Send Message' class="btn-main">
      </div>

      <div id="success_message" class='success'>
        Your message has been sent successfully. Refresh this page if you want to send more messages.
      </div>
      <div id="error_message" class='error'>
        Sorry there was an error sending your form.
      </div>

    </div>
  </form>
</template>

<script>
export default {
  name: "ContactForm"
}
</script>

<style scoped>

</style>
