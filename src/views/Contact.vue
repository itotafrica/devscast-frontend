<template>
<div class="contact">

  <PageHeader name="Contact Us"></PageHeader>

  <main class="main" id="main">
    <section class="section-negative">
      <div class="container">

        <!-- ===== PAGE CONTENT ===== -->
        <div class="page-content mt-60">

          <!-- ===== PAGE TITLE & DESCRIPTION ===== -->
          <div class="row">
            <div class="col-md-8 col-md-offset-2 text-center">
              <h2 class="title-default mb-10">Get in touch</h2>
              <p class="page-description mb-70">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Maiores atque, officia molestias, vel nulla consectetur asperiores fugit quas voluptate eaque amet quasi id ipsum cupiditate, illo placeat distinctio optio aliquam.</p>
            </div>
          </div>

          <!-- ===== FORM CONTACT ===== -->
          <div class="row">
            <div class="col-md-8 col-md-offset-2">
              <form action="php/contact.php" method="POST" id="form-contact" class="form-contact form-validate">
                <fieldset>
                  <div class="mb-20">
                    <label for="name" class="label-control">Name* :</label>
                    <input type="text" name="name" class="form-control" id="name" required />
                  </div>
                  <div class="mb-20">
                    <label for="email" class="label-control">Email* :</label>
                    <input type="email" name="email" class="form-control" id="email" required />
                  </div>
                  <div class="mb-20">
                    <label for="subject" class="label-control">Subject* :</label>
                    <input type="text" name="subject" class="form-control" id="subject" required />
                  </div>
                  <div class="mb-20">
                    <label for="message" class="label-control">Message* :</label>
                    <textarea name="message" id="message" rows="6" class="form-control" required></textarea>
                  </div>
                  <div class="mb-20 text-right">
                    <input type="submit" class="btn btn-success btn-lg" value="Submit" />
                  </div>
                  <div class="form-callback success">
                    <p>Success! Thank you for contact us.</p>
                  </div>
                  <div class="form-callback error">
                    <p>Error! Something went wrong.</p>
                  </div>
                </fieldset>
              </form>
            </div>
          </div>
        </div>

      </div>
    </section>

    <div class="map" id="map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d15630.679180929914!2d27.4688104!3d-11.6468624!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x51540f372bd869d6!2sNgpictures!5e0!3m2!1sfr!2scd!4v1545836979670" frameborder="0" style="border:0" allowfullscreen></iframe>
    </div>

    <DonateSection></DonateSection>
  </main>
</div>
</template>

<script>
import PageHeader from '@/components/PageHeader.vue'
import DonateSection from '@/components/Sections/DonateSection.vue'

export default {
  name: 'Contact',
  components: {
    PageHeader,
    DonateSection
  }
}
</script>
