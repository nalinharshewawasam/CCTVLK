<template>
  <q-page class="bg-grey-1">
    <!-- Hero Slider Section -->
    <div class="hero-slider-container">
      <q-carousel
        animated
        v-model="slide"
        navigation
        infinite
        :autoplay="autoplay"
        arrows
        @mouseenter="autoplay = false"
        @mouseleave="autoplay = true"
        height="500px"
        class="bg-grey-9 text-white shadow-2"
      >
        <q-carousel-slide name="first" img-src="https://cdn.quasar.dev/img/parallax2.jpg">
          <div class="absolute-full flex flex-center custom-caption">
            <div class="text-center">
              <div class="text-h2 text-weight-bold q-mb-sm text-shadow">Smart Security</div>
              <div class="text-h5 text-grey-2 q-mb-lg text-shadow">
                Protect your home with advanced AI detection
              </div>
              <q-btn
                color="primary"
                label="Shop Now"
                unelevated
                rounded
                size="lg"
                icon-right="arrow_forward"
              />
            </div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide name="second" img-src="https://cdn.quasar.dev/img/parallax1.jpg">
          <div class="absolute-full flex flex-center custom-caption">
            <div class="text-center">
              <div class="text-h2 text-weight-bold q-mb-sm text-shadow">Business Solutions</div>
              <div class="text-h5 text-grey-2 q-mb-lg text-shadow">
                Complete coverage for offices
              </div>
              <q-btn
                color="white"
                text-color="dark"
                label="View Solutions"
                unelevated
                rounded
                size="lg"
              />
            </div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide name="third" img-src="https://cdn.quasar.dev/img/mountains.jpg">
          <div class="absolute-full flex flex-center custom-caption">
            <div class="text-center">
              <div class="text-h2 text-weight-bold q-mb-sm text-shadow">24/7 Monitoring</div>
              <div class="text-h5 text-grey-2 q-mb-lg text-shadow">
                Stay connected from anywhere
              </div>
              <q-btn outline color="white" label="Learn More" rounded size="lg" />
            </div>
          </div>
        </q-carousel-slide>
      </q-carousel>
    </div>

    <!-- 3 Main Categories -->
    <div
      class="q-pa-md max-width-container q-mx-auto q-mt-md"
      style="position: relative; z-index: 10"
    >
      <div class="row q-col-gutter-lg">
        <!-- WI-FI CAMERA -->
        <div class="col-12 col-md-4">
          <q-card
            class="category-banner bg-white cursor-pointer hover-zoom overflow-hidden shadow-3"
          >
            <q-img
              src="https://cdn.quasar.dev/img/parallax1.jpg"
              :ratio="16 / 9"
              style="height: 220px"
            >
              <div class="absolute-full flex flex-center banner-overlay">
                <div class="text-center">
                  <q-icon name="wifi" size="3em" color="white" class="q-mb-sm" />
                  <div class="text-h5 text-weight-bold text-uppercase tracking-wide text-white">
                    WI-FI CAMERA
                  </div>
                  <div class="text-caption text-grey-3 q-mt-xs">Wireless & Easy Setup</div>
                </div>
              </div>
            </q-img>
          </q-card>
        </div>

        <!-- CCTV PACKAGES -->
        <div class="col-12 col-md-4">
          <q-card
            class="category-banner bg-white cursor-pointer hover-zoom overflow-hidden shadow-3"
          >
            <q-img
              src="https://cdn.quasar.dev/img/parallax2.jpg"
              :ratio="16 / 9"
              style="height: 220px"
            >
              <div class="absolute-full flex flex-center banner-overlay">
                <div class="text-center">
                  <q-icon name="inventory_2" size="3em" color="white" class="q-mb-sm" />
                  <div class="text-h5 text-weight-bold text-uppercase tracking-wide text-white">
                    CCTV PACKAGES
                  </div>
                  <div class="text-caption text-grey-3 q-mt-xs">Complete Kits for Home</div>
                </div>
              </div>
            </q-img>
          </q-card>
        </div>

        <!-- SPECIAL OFFERS -->
        <div class="col-12 col-md-4">
          <q-card
            class="category-banner bg-white cursor-pointer hover-zoom overflow-hidden shadow-3"
          >
            <q-img
              src="https://cdn.quasar.dev/img/mountains.jpg"
              :ratio="16 / 9"
              style="height: 220px"
            >
              <div class="absolute-full flex flex-center banner-overlay">
                <div class="text-center">
                  <q-icon name="local_offer" size="3em" color="warning" class="q-mb-sm" />
                  <div class="text-h5 text-weight-bold text-uppercase tracking-wide text-white">
                    SPECIAL OFFERS
                  </div>
                  <div class="text-caption text-grey-3 q-mt-xs">Limited Time Deals</div>
                </div>
              </div>
            </q-img>
          </q-card>
        </div>
      </div>
    </div>

    <!-- Best Sellers -->
    <div class="bg-white q-py-xl q-mt-lg">
      <div class="max-width-container q-mx-auto q-px-md">
        <div class="text-center q-mb-xl">
          <div class="text-h3 text-weight-bold text-blue-grey-10">Best Selling Products</div>
          <div class="text-subtitle1 text-grey-6 q-mt-sm">
            Top rated security solutions chosen by our customers
          </div>
        </div>

        <div class="row q-col-gutter-lg">
          <div class="col-12 col-sm-6 col-md-3" v-for="product in products" :key="product.id">
            <q-card class="product-card column full-height no-wrap" flat bordered>
              <div class="relative-position">
                <!-- Use placehold.co for reliable placeholders -->
                <q-img :src="product.image" :ratio="1" contain class="q-pa-md bg-grey-1" />
                <q-chip
                  v-if="product.tag"
                  :color="product.tagColor || 'primary'"
                  text-color="white"
                  class="absolute-top-left q-ma-sm"
                  dense
                  size="sm"
                >
                  {{ product.tag }}
                </q-chip>
                <q-btn
                  round
                  color="white"
                  text-color="grey-9"
                  icon="favorite_border"
                  class="absolute-top-right q-ma-sm shadow-1"
                  size="sm"
                />
              </div>

              <q-card-section class="col-grow">
                <div class="text-caption text-grey-6 q-mb-xs">{{ product.brand }}</div>
                <div
                  class="text-subtitle1 text-weight-bold text-blue-grey-10 ellipsis-2-lines line-clamp-2"
                  style="height: 48px"
                >
                  {{ product.name }}
                </div>
                <div class="row items-center q-mt-sm">
                  <q-rating :model-value="product.rating" size="1em" color="warning" readonly />
                  <span class="text-caption text-grey-6 q-ml-sm">({{ product.reviews }})</span>
                </div>
              </q-card-section>

              <q-card-section class="q-pt-none">
                <div class="text-h5 text-primary text-weight-bold">Rs. {{ product.price }}</div>
              </q-card-section>

              <q-separator />
              <q-btn
                flat
                class="full-width q-py-md text-weight-bold"
                color="primary"
                label="Add to Cart"
                icon="shopping_cart"
              />
            </q-card>
          </div>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const slide = ref('first')
const autoplay = ref(true)

const products = ref([
  {
    id: 1,
    name: 'Hikvision 2MP 1080p Dome Camera Night Vision',
    brand: 'HIKVISION',
    price: '4,500',
    rating: 4.5,
    reviews: 24,
    image: 'https://placehold.co/400x400/f5f5f5/333?text=Dome+Cam',
    tag: 'Best Seller',
    tagColor: 'orange',
  },
  {
    id: 2,
    name: 'Dahua 5MP Outdoor Bullet Camera Waterproof IP67',
    brand: 'DAHUA',
    price: '6,200',
    rating: 5,
    reviews: 10,
    image: 'https://placehold.co/400x400/f5f5f5/333?text=Bullet+Cam',
    tag: 'New',
    tagColor: 'green',
  },
  {
    id: 3,
    name: 'EZVIZ C6N 360 Degree Smart WiFi Camera',
    brand: 'EZVIZ',
    price: '8,900',
    rating: 4,
    reviews: 56,
    image: 'https://placehold.co/400x400/f5f5f5/333?text=WiFi+Cam',
  },
  {
    id: 4,
    name: '8 Channel DVR 1080p H.265+ Support',
    brand: 'HIKVISION',
    price: '14,500',
    rating: 4.5,
    reviews: 8,
    image: 'https://placehold.co/400x400/f5f5f5/333?text=DVR',
  },
])
</script>

<style>
/* Standard CSS */

.custom-caption {
  text-align: center;
  padding: 12px;
  color: white;
  background-color: rgba(0, 0, 0, 0.4);
}

.text-shadow {
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.6);
}

.max-width-container {
  max-width: 1200px;
}

.banner-overlay {
  background: rgba(13, 71, 161, 0.7); /* Primary Blue Overlay with opacity */
  transition: background 0.3s;
}

.hover-zoom:hover .banner-overlay {
  background: rgba(13, 71, 161, 0.85);
}

.hover-zoom .q-img__image {
  transition: transform 0.5s ease;
}

.hover-zoom:hover .q-img__image {
  transform: scale(1.1);
}

.product-card {
  transition: all 0.3s;
  border-radius: 12px;
}
.product-card:hover {
  border-color: #1976d2;
  box-shadow: 0 4px 15px rgba(25, 118, 210, 0.15);
}

.tracking-wide {
  letter-spacing: 0.1em;
}
</style>
