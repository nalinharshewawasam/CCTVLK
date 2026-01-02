<template>
  <q-page class="bg-grey-1">
    <!-- Hero Section -->
    <div class="about-hero shadow-2 relative-position overflow-hidden">
      <q-img
        src="https://cdn.pixabay.com/photo/2016/11/29/09/32/concept-1868728_1280.jpg"
        class="full-width full-height dimmed-bg"
        fit="cover"
      >
        <div class="absolute-full flex flex-center column text-white">
          <div
            class="text-h2 text-weight-bold text-uppercase tracking-wider q-mb-sm text-center animate-fade-up"
          >
            About Us
          </div>
          <div class="text-h5 text-weight-light text-center q-px-md animate-fade-up delay-200">
            The Trusted Security Solutions Provider in Sri Lanka
          </div>
        </div>
      </q-img>
    </div>

    <div class="q-pa-md max-width-container q-mx-auto q-mt-xl">
      <!-- Our Story -->
      <div class="row q-col-gutter-xl items-center q-mb-xl section-fade">
        <div class="col-12 col-md-6">
          <div class="text-overline text-primary text-weight-bold q-mb-sm">OUR STORY</div>
          <div class="text-h4 text-blue-grey-10 text-weight-bold q-mb-md">
            Building a Safer Sri Lanka Since 2015
          </div>
          <p class="text-body1 text-grey-8 leading-relaxed">
            Originating as a proud subsidiary of <strong>NEKZONE SOLUTIONS PVT Ltd</strong>, CCTV.LK
            has successfully fortified its position in Sri Lanka’s security landscape for over eight
            years. Our mission has been clear: to provide top-notch security solutions ensuring
            robust protection for individuals, businesses, and communities.
          </p>
        </div>
        <div class="col-12 col-md-6">
          <q-img
            src="https://cdn.pixabay.com/photo/2014/05/02/21/49/home-office-336373_640.jpg"
            class="rounded-borders shadow-4 hover-scale"
          />
        </div>
      </div>

      <!-- Partnerships -->
      <div class="q-mb-xl section-fade">
        <div class="text-center q-mb-lg">
          <div class="text-h4 text-blue-grey-10 text-weight-bold">Partnerships & Credentials</div>
          <div
            class="q-separator bg-primary q-mx-auto q-mt-md"
            style="width: 60px; height: 4px"
          ></div>
        </div>

        <div class="row q-col-gutter-lg">
          <div class="col-12 col-md-4">
            <q-card class="full-height text-center q-pa-md hover-lift">
              <q-card-section>
                <q-icon name="verified_user" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">
                  Authorized Affiliations
                </div>
                <p class="text-grey-7">
                  As certified partners of globally renowned brands – Dahua, Hikvision, and Uniview,
                  we pledge quality and reliability in every product.
                </p>
              </q-card-section>
            </q-card>
          </div>
          <div class="col-12 col-md-4">
            <q-card class="full-height text-center q-pa-md hover-lift">
              <q-card-section>
                <q-icon name="public" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">
                  Locally Sourced, Globally Recognized
                </div>
                <p class="text-grey-7">
                  We prioritize local suppliers within Sri Lanka, ensuring the authenticity and
                  genuine quality of each product.
                </p>
              </q-card-section>
            </q-card>
          </div>
          <div class="col-12 col-md-4">
            <q-card class="full-height text-center q-pa-md hover-lift">
              <q-card-section>
                <q-icon name="build_circle" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">
                  Assured Warranty & Support
                </div>
                <p class="text-grey-7">
                  Each product comes with a 2-year warranty and unmatched technical support,
                  reflecting our commitment to you.
                </p>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>

      <!-- Why Us (Timeline or List style) -->
      <div class="bg-white q-pa-xl rounded-borders shadow-1 q-mb-xl section-fade">
        <div class="text-h4 text-blue-grey-10 text-weight-bold q-mb-xl text-center">
          Why CCTV.LK Stands Out
        </div>

        <div class="row q-col-gutter-xl">
          <div class="col-12 col-md-6">
            <q-list padding>
              <q-item>
                <q-item-section avatar>
                  <q-icon name="star" color="orange" size="lg" />
                </q-item-section>
                <q-item-section>
                  <q-item-label class="text-h6 text-weight-bold">Industry Reputation</q-item-label>
                  <q-item-label caption class="text-body1 text-grey-8"
                    >Cultivated a stellar reputation by continuously offering outstanding technical
                    support and customer service.</q-item-label
                  >
                </q-item-section>
              </q-item>

              <q-item class="q-mt-md">
                <q-item-section avatar>
                  <q-icon name="check_circle" color="green" size="lg" />
                </q-item-section>
                <q-item-section>
                  <q-item-label class="text-h6 text-weight-bold"
                    >Genuine Products Guarantee</q-item-label
                  >
                  <q-item-label caption class="text-body1 text-grey-8"
                    >We only stock branded and genuine equipment, giving you confidence in
                    authenticity.</q-item-label
                  >
                </q-item-section>
              </q-item>

              <q-item class="q-mt-md">
                <q-item-section avatar>
                  <q-icon name="settings_suggest" color="blue" size="lg" />
                </q-item-section>
                <q-item-section>
                  <q-item-label class="text-h6 text-weight-bold"
                    >Tailored Security Solutions</q-item-label
                  >
                  <q-item-label caption class="text-body1 text-grey-8"
                    >Adept at consulting and providing solutions tailored to your unique
                    requirements.</q-item-label
                  >
                </q-item-section>
              </q-item>
            </q-list>
          </div>

          <div class="col-12 col-md-6">
            <q-img
              src="https://cdn.pixabay.com/photo/2018/01/20/08/33/cctv-3094056_640.jpg"
              class="rounded-borders full-height"
              style="min-height: 300px"
              fit="cover"
            />
          </div>
        </div>
      </div>

      <!-- Detailed Info Grid -->
      <div class="row q-col-gutter-lg q-mb-xl section-fade">
        <div class="col-12 col-md-6">
          <q-card class="bg-blue-grey-9 text-white full-height q-pa-lg">
            <div class="text-h5 text-weight-bold q-mb-md row items-center">
              <q-icon name="store" class="q-mr-sm" /> Our Physical Presence & Expertise
            </div>
            <p class="text-body1 leading-relaxed text-grey-4">
              Located in the heart of Aturugiriya, Colombo, our Head Office and primary showroom
              welcomes visitors to explore our offerings. Beyond selling, our in-house team of adept
              security technicians is geared up to deliver expert installation services, ensuring
              operational efficiency at competitive prices.
            </p>
          </q-card>
        </div>
        <div class="col-12 col-md-6">
          <q-card class="bg-primary text-white full-height q-pa-lg">
            <div class="text-h5 text-weight-bold q-mb-md row items-center">
              <q-icon name="school" class="q-mr-sm" /> Guidance for Online Buyers
            </div>
            <p class="text-body1 leading-relaxed text-blue-1">
              While purchasing online can be cost-effective, understanding the nuances of security
              product installation and configuration is crucial. To bridge this gap, we offer both
              guidance and professional installation services, ensuring a seamless experience from
              purchase to setup.
            </p>
          </q-card>
        </div>
      </div>

      <!-- Bottom Legacy -->
      <div class="text-center q-mb-xl q-px-md section-fade">
        <div class="text-h4 text-blue-grey-10 text-weight-bold q-mb-lg">
          Our Legacy and Commitment
        </div>
        <p class="text-body1 text-grey-8 text-center max-width-text q-mx-auto">
          Established in 2015, CCTV.LK’s commitment to Sri Lanka’s security needs has been
          unwavering. As a testament to our dedication to value, if you ever find a product we stock
          at a cheaper rate elsewhere, let us know. We promise not just to match but strive to beat
          that price.
        </p>
        <div class="text-h6 text-primary q-mt-lg text-weight-medium">
          Your safety and satisfaction stand at the core of our operations at CCTV.LK. Partner with
          us for a secure, protected future.
        </div>
      </div>

      <!-- Expertise & Products Block -->
      <div class="row q-col-gutter-xl q-mb-xl section-fade">
        <div class="col-12 col-md-6">
          <div class="text-h5 text-blue-grey-9 text-weight-bold q-mb-md">Our Expertise</div>
          <p class="text-body1 text-grey-8">
            With years of dedicated service in the industry, we have honed our expertise in
            designing, implementing, and maintaining high-quality CCTV systems. Our team of seasoned
            professionals brings a wealth of knowledge and hands-on experience to the table,
            ensuring that your security needs are met with tailor-made solutions.
          </p>
        </div>
        <div class="col-12 col-md-6">
          <div class="text-h5 text-blue-grey-9 text-weight-bold q-mb-md">Our Products</div>
          <p class="text-body1 text-grey-8">
            At CCTV.lk, we offer an extensive range of CCTV cameras and accessories sourced from
            renowned brands that are known for their reliability and advanced technology. From
            state-of-the-art IP cameras to traditional analog cameras, we have a diverse selection
            to cater to various surveillance needs.
          </p>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
// No script needed for static content
</script>

<style scoped>
.about-hero {
  height: 400px;
}

.dimmed-bg::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(10, 25, 41, 0.7); /* Dark Blue overlay */
  z-index: 1;
}

.tracking-wider {
  letter-spacing: 2px;
}

.max-width-container {
  max-width: 1200px;
}

.max-width-text {
  max-width: 800px;
}

.leading-relaxed {
  line-height: 1.8;
}

/* Animations */
.animate-fade-up {
  animation: fadeUp 1s ease-out forwards;
  opacity: 0;
  transform: translateY(20px);
}

.delay-200 {
  animation-delay: 0.2s;
}

@keyframes fadeUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.hover-lift {
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
  border-radius: 12px;
}
.hover-lift:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.hover-scale {
  transition: transform 0.4s ease;
}
.hover-scale:hover {
  transform: scale(1.02);
}
</style>
