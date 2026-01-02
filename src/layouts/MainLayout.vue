<template>
  <q-layout view="lHh Lpr lff" class="bg-grey-1">
    <!-- Header: Blue for security theme -->
    <q-header elevated class="bg-primary text-white">
      <!-- Top Bar -->
      <div class="bg-blue-grey-10 text-white q-py-xs q-px-md text-caption">
        <div class="row justify-between items-center" style="max-width: 1400px; margin: 0 auto">
          <div class="row q-gutter-x-lg">
            <div class="row items-center hover-text-grey">
              <q-icon name="phone" size="14px" class="q-mr-xs" />
              <span>+94 71 8000 300</span>
            </div>
            <div class="row items-center hover-text-grey">
              <q-icon name="email" size="14px" class="q-mr-xs" />
              <span>sales@cctv.lk</span>
            </div>
          </div>
          <q-btn
            flat
            dense
            no-caps
            size="sm"
            icon="lock"
            label="Partner Portal Login"
            class="text-white"
          />
        </div>
      </div>

      <q-toolbar class="q-py-sm">
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
          class="q-mr-sm lt-md"
        />

        <router-link to="/" class="q-mr-md flex flex-center" style="text-decoration: none">
          <img
            src="../assets/cctv-logo.png"
            alt="CCTVLK Logo"
            style="height: 32px; max-width: 200px; object-fit: contain"
          />
        </router-link>

        <q-space />

        <!-- Desktop Navigation -->
        <div class="gt-sm row items-center q-gutter-x-sm">
          <q-btn stretch flat class="nav-btn" label="HOME" to="/" />
          <q-btn stretch flat class="nav-btn" label="PRODUCTS & SOLUTIONS" />
          <q-btn stretch flat class="nav-btn" label="TECHNICAL SUPPORT" to="/support" />
          <q-btn stretch flat class="nav-btn" label="OUR PROJECTS" />
          <q-btn stretch flat class="nav-btn" label="ABOUT US" to="/about" />
        </div>

        <q-space />

        <div class="row items-center q-gutter-sm">
          <q-btn flat round color="white" icon="search" />
          <q-btn flat round color="white" icon="shopping_cart">
            <q-badge color="red" floating>2</q-badge>
          </q-btn>
          <q-btn
            unelevated
            rounded
            color="white"
            text-color="primary"
            label="Login"
            class="q-px-md gt-xs"
            no-caps
          />
          <q-btn flat round color="white" icon="person" class="lt-sm" />
        </div>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" bordered class="bg-white" :width="280">
      <div class="q-pa-md column flex-center bg-blue-grey-1">
        <q-icon name="security" size="4em" color="primary" class="q-mb-sm" />
        <div class="text-h6 text-primary text-weight-bold">CCTVLK</div>
        <div class="text-caption text-grey-7">Security Solutions</div>
      </div>

      <q-list padding class="text-grey-8">
        <q-item clickable v-ripple to="/" active-class="text-primary bg-blue-1">
          <q-item-section avatar>
            <q-icon name="home" />
          </q-item-section>
          <q-item-section>Home</q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="inventory_2" />
          </q-item-section>
          <q-item-section>Products & Solutions</q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="support_agent" />
          </q-item-section>
          <q-item-section>Technical Support</q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="engineering" />
          </q-item-section>
          <q-item-section>Our Projects</q-item-section>
        </q-item>

        <q-separator class="q-my-md" />

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="info" />
          </q-item-section>
          <q-item-section>About Us</q-item-section>
        </q-item>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <!-- Footer -->
    <q-footer class="bg-blue-grey-10 text-grey-4">
      <div class="max-width-container q-mx-auto">
        <div class="row q-col-gutter-xl q-pa-xl">
          <div class="col-12 col-md-4">
            <div class="row items-center q-mb-md">
              <q-icon name="videocam" size="2em" class="text-white q-mr-sm" />
              <span class="text-h5 text-white text-weight-bold">CCTVLK</span>
            </div>
            <p class="text-body2 leading-relaxed">
              We provide state-of-the-art security systems for homes and businesses. Trust us to
              keep your world secure with advanced technology and reliable monitoring.
            </p>
            <div class="row q-gutter-sm q-mt-md">
              <q-btn round flat size="sm" icon="facebook" class="bg-blue-grey-9 text-white" />
              <q-btn round flat size="sm" icon="rss_feed" class="bg-blue-grey-9 text-white" />
              <q-btn round flat size="sm" icon="camera_alt" class="bg-blue-grey-9 text-white" />
            </div>
          </div>

          <div class="col-12 col-sm-6 col-md-4">
            <div class="text-h6 text-white q-mb-md">Quick Links</div>
            <div class="column q-gutter-y-sm">
              <a href="#" class="footer-link">Smart Cameras</a>
              <a href="#" class="footer-link">Wireless Systems</a>
              <a href="#" class="footer-link">Installation Services</a>
              <a href="#" class="footer-link">Warranty Support</a>
            </div>
          </div>

          <div class="col-12 col-sm-6 col-md-4">
            <div class="text-h6 text-white q-mb-md">Contact Us</div>
            <div class="q-gutter-y-md">
              <div class="row items-start">
                <q-icon name="location_on" size="sm" class="q-mr-md text-primary q-mt-xs" />
                <div>
                  <div class="text-white text-weight-bold">ADDRESS:</div>
                  <div class="text-caption text-grey-4">
                    Nekzone Solutions (Pvt)Ltd,<br />
                    401/8, Godagama Road,<br />
                    Habarakada.
                  </div>
                </div>
              </div>

              <div class="row items-center">
                <q-icon name="phone" size="sm" class="q-mr-md text-primary" />
                <div>
                  <div class="text-white text-weight-bold">PHONE:</div>
                  <div class="text-caption text-grey-4">+94 71 8000 300</div>
                </div>
              </div>

              <div class="row items-center">
                <q-icon name="email" size="sm" class="q-mr-md text-primary" />
                <div>
                  <div class="text-white text-weight-bold">EMAIL:</div>
                  <div class="text-caption text-grey-4">sales@cctv.lk</div>
                </div>
              </div>

              <div class="row items-center">
                <q-icon name="schedule" size="sm" class="q-mr-md text-primary" />
                <div>
                  <div class="text-white text-weight-bold">WORKING DAYS/HOURS:</div>
                  <div class="text-caption text-grey-4">Mon - Sun / 9:00 AM - 8:00 PM</div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <q-separator color="blue-grey-9" />

        <div class="row justify-between items-center q-pa-md text-caption">
          <div>&copy; 2024 CCTVLK. All Rights Reserved.</div>
          <div class="row q-gutter-x-md">
            <router-link to="/policy" class="text-grey-4 text-decoration-none hover-text-white"
              >Privacy Policy</router-link
            >
            <span class="cursor-pointer hover-text-white">Terms of Service</span>
          </div>
        </div>
      </div>
    </q-footer>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'

const leftDrawerOpen = ref(false)

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value
}
</script>

<style>
/* Standard CSS - No SCSS nesting */

/* Navigation Button Hover Effect */
.nav-btn {
  font-weight: 500;
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
  position: relative;
  overflow: visible; /* Allow ::after to be seen if outside */
}

.nav-btn::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(255, 255, 255, 0.1);
  transform: scaleY(0);
  transform-origin: bottom;
  transition: transform 0.3s ease;
  border-radius: 4px;
}

.nav-btn:hover::before {
  transform: scaleY(1);
}

.nav-btn::after {
  content: '';
  position: absolute;
  bottom: 2px;
  left: 50%;
  width: 0;
  height: 2px;
  background-color: #ffffff;
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  box-shadow: 0 0 5px rgba(255, 255, 255, 0.8);
}

.nav-btn:hover::after {
  width: 80%;
  left: 10%;
}

.footer-link {
  color: #b0bec5;
  text-decoration: none;
  transition: color 0.3s;
}
.footer-link:hover {
  color: white;
}
.hover-text-white:hover {
  color: white;
}
.max-width-container {
  max-width: 1400px;
}
.leading-relaxed {
  line-height: 1.6;
}
</style>
