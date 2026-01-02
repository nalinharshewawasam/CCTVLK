<template>
  <q-page class="bg-grey-1">
    <!-- Hero Section -->
    <div
      class="support-hero shadow-2 relative-position overflow-hidden flex flex-center"
      style="
        background: url('https://images.unsplash.com/photo-1517048676732-d65bc937f952?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80')
          center center / cover no-repeat;
      "
    >
      <!-- Dark Overlay -->
      <div class="absolute-full" style="background: rgba(10, 25, 41, 0.75); z-index: 1"></div>

      <!-- Content -->
      <div
        class="relative-position column flex-center text-white text-center q-px-md"
        style="z-index: 2"
      >
        <div class="text-h2 text-weight-bold text-uppercase tracking-wider q-mb-sm">
          Technical Support
        </div>
        <div class="text-h5 text-weight-light">We are here to help, 24/7</div>
      </div>
    </div>

    <div class="q-pa-md max-width-container q-mx-auto q-mt-xl">
      <!-- Top Contact Block -->
      <div class="text-center q-mb-xl section-fade">
        <div class="text-h4 text-blue-grey-10 text-weight-bold q-mb-md">
          Contact our Technical Support Team
        </div>
        <div class="row justify-center q-gutter-x-xl q-mt-lg">
          <div class="row items-center">
            <q-icon name="phone" color="primary" size="2em" class="q-mr-sm" />
            <div class="text-h5 text-grey-8">+94 71 8000 300</div>
          </div>
          <div class="row items-center">
            <q-icon name="email" color="primary" size="2em" class="q-mr-sm" />
            <div class="text-h5 text-grey-8">info@cctv.lk</div>
          </div>
        </div>
      </div>

      <!-- Introduction -->
      <div class="q-mb-xl section-fade text-center max-width-text q-mx-auto">
        <p class="text-body1 text-grey-8 leading-relaxed">
          At CCTV.LK, our relationship with our clients extends far beyond the point of sale. Our
          dedication to your security doesn’t end when you leave our showroom or website; it’s just
          the beginning.
        </p>
      </div>

      <!-- Assistance Options Grid -->
      <div class="q-mb-xl section-fade">
        <div class="text-h4 text-center text-blue-grey-10 text-weight-bold q-mb-xl">
          Need Assistance? We’re Here to Help!
        </div>
        <div class="row q-col-gutter-lg">
          <div class="col-12 col-md-4">
            <q-card class="full-height hover-lift">
              <q-card-section class="text-center q-pa-lg">
                <q-icon name="support_agent" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">
                  24/7 Support Line
                </div>
                <p class="text-grey-7">
                  Our hotline is available round-the-clock. Simply call us at
                  <strong>+94 71 8000 300</strong> for immediate assistance.
                </p>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-4">
            <q-card class="full-height hover-lift">
              <q-card-section class="text-center q-pa-lg">
                <q-icon name="mail" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">Email Support</div>
                <p class="text-grey-7">
                  Prefer to detail your issue in writing? Send us an email at
                  <strong>info@cctv.lk</strong> and we will provide detailed instructions.
                </p>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-4">
            <q-card class="full-height hover-lift">
              <q-card-section class="text-center q-pa-lg">
                <q-icon name="assignment" size="4em" color="primary" class="q-mb-md" />
                <div class="text-h6 text-weight-bold text-blue-grey-9 q-mb-sm">
                  Online Support Form
                </div>
                <p class="text-grey-7">
                  For less urgent inquiries, fill out our online support form. Our team will
                  coordinate with you efficiently.
                </p>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-6">
            <q-card class="full-height hover-lift bg-blue-grey-1">
              <q-card-section class="row items-center q-pa-lg">
                <div class="col-auto q-mr-md">
                  <q-icon name="laptop_mac" size="3em" color="blue-grey-9" />
                </div>
                <div class="col">
                  <div class="text-h6 text-weight-bold text-blue-grey-9">Remote Assistance</div>
                  <p class="text-grey-8 q-mb-none">
                    Issues can often be resolved remotely. Our technicians can guide you through
                    steps or access your system remotely.
                  </p>
                </div>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-6">
            <q-card class="full-height hover-lift bg-blue-grey-1">
              <q-card-section class="row items-center q-pa-lg">
                <div class="col-auto q-mr-md">
                  <q-icon name="engineering" size="3em" color="blue-grey-9" />
                </div>
                <div class="col">
                  <div class="text-h6 text-weight-bold text-blue-grey-9">
                    On-Site Technical Service
                  </div>
                  <p class="text-grey-8 q-mb-none">
                    If needed, our skilled technicians will visit your location with the necessary
                    tools to resolve any issue.
                  </p>
                </div>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>

      <!-- Resources Section -->
      <div class="bg-white rounded-borders shadow-1 q-pa-xl q-mb-xl section-fade">
        <div class="text-h4 text-center text-blue-grey-10 text-weight-bold q-mb-lg">
          Resources at Your Fingertips
        </div>
        <div class="row q-col-gutter-xl text-center">
          <div class="col-6 col-md-3">
            <q-btn round color="primary" icon="description" size="xl" class="q-mb-sm shadow-3" />
            <div class="text-subtitle1 text-weight-bold">Installation Guides</div>
            <div class="text-caption text-grey-6">Step-by-step walkthroughs</div>
          </div>

          <div class="col-6 col-md-3">
            <q-btn round color="primary" icon="help" size="xl" class="q-mb-sm shadow-3" />
            <div class="text-subtitle1 text-weight-bold">FAQs</div>
            <div class="text-caption text-grey-6">Quick fixes & advice</div>
          </div>

          <div class="col-6 col-md-3">
            <q-btn round color="primary" icon="menu_book" size="xl" class="q-mb-sm shadow-3" />
            <div class="text-subtitle1 text-weight-bold">Product Manuals</div>
            <div class="text-caption text-grey-6">Detailed information</div>
          </div>

          <div class="col-6 col-md-3">
            <q-btn round color="primary" icon="play_circle" size="xl" class="q-mb-sm shadow-3" />
            <div class="text-subtitle1 text-weight-bold">Tutorial Videos</div>
            <div class="text-caption text-grey-6">Setup & Config</div>
          </div>
        </div>
      </div>

      <!-- Bottom Call to Action -->
      <div class="bg-primary text-white text-center q-pa-xl rounded-borders section-fade">
        <div class="text-h4 text-weight-bold q-mb-md">Committed to Your Peace of Mind</div>
        <p class="text-body1 text-grey-3 max-width-text q-mx-auto q-mb-lg">
          Our technical support is a reflection of our commitment to you and your safety. At
          CCTV.LK, we don’t just provide products; we deliver solutions and support to ensure that
          those solutions remain effective and reliable.
        </p>
        <div class="text-h5 text-weight-medium q-mb-md">We’re Only a Call or Click Away</div>
        <q-btn outline color="white" label="Contact Us Now" size="lg" to="/contact" />
        <div class="q-mt-lg text-caption">
          Partner with CCTV.LK for uninterrupted safety and unrivaled support
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
// Static content
</script>

<style scoped>
.support-hero {
  height: 350px;
}

.dimmed-bg::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(10, 25, 41, 0.75);
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

.hover-lift {
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
  border-radius: 12px;
}
.hover-lift:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
}
</style>
