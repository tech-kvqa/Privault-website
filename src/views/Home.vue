<!-- <template>
  <v-container>
    <h2>Privalut Website</h2>
  </v-container>
</template>

<script>
</script> -->


<!-- <template>
  <v-container class="fill-height text-center">
    <v-row align="center" justify="center">
      <v-col>
        <h1 class="text-h2 mb-4" data-aos="fade-up">Cybersecurity Redefined</h1>
        <p data-aos="fade-in" data-aos-delay="200">Your digital shield against modern threats.</p>
        <v-btn color="primary" large data-aos="zoom-in" data-aos-delay="400">Explore Now</v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>
 -->


<!-- <template>
  <v-container fluid class="pa-0">
    <v-container class="fill-height text-center hero-section" id="hero">
      <v-row align="center" justify="center">
        <v-col>
          <h1 class="text-h2 mb-4 text-white" data-aos="fade-up">Cybersecurity Redefined</h1>
          <p class="text-white" data-aos="fade-in" data-aos-delay="200">Your digital shield against modern threats.</p>
          <v-btn
            color="primary"
            size="large"
            class="mt-4"
            data-aos="zoom-in"
            data-aos-delay="400"
            @click="scrollToProducts"
          >
            Explore Now
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    <v-container id="products" class="mt-12 mb-16">
      <h2 class="text-center mb-10" data-aos="fade-up">Our Product Suite</h2>
      <v-row dense>
        <v-col
          v-for="product in products"
          :key="product.title"
          cols="12"
          md="4"
          class="mb-6"
          data-aos="fade-up"
          data-aos-delay="200"
        >
          <v-card class="pa-4 text-center" color="#1f3557" dark>
            <v-icon size="40" class="mb-3">{{ product.icon }}</v-icon>
            <h3 class="text-h6 mb-2">{{ product.title }}</h3>
            <p class="text-body-2 mb-3">{{ product.description }}</p>
            <v-btn color="primary" :to="product.route" variant="outlined">Learn More</v-btn>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          title: 'Compliance Metrics',
          route: '/product/compliance-metrics',
          description: 'Track privacy KPIs, audits, data health, and regulatory status.',
          icon: 'mdi-chart-bar'
        },
        {
          title: 'Breach Management',
          route: '/product/breach-management',
          description: 'Detect, document, and act swiftly on data breaches.',
          icon: 'mdi-shield-alert'
        },
        {
          title: 'DPIA (Risk Assessment)',
          route: '/product/dpia',
          description: 'Assess and mitigate privacy risks across systems and vendors.',
          icon: 'mdi-clipboard-alert'
        },
        {
          title: 'Governance',
          route: '/product/governance',
          description: 'Centralize your privacy framework and organizational controls.',
          icon: 'mdi-account-group'
        },
        {
          title: 'DSR Management',
          route: '/product/dsr-management',
          description: 'Automate and fulfill Data Subject Requests efficiently.',
          icon: 'mdi-account-key'
        },
        {
          title: 'Vendor Management',
          route: '/product/vendor-management',
          description: 'Track and assess third-party compliance and contracts.',
          icon: 'mdi-truck'
        },
        {
          title: 'Phishing App',
          route: '/product/phishing-app',
          description: 'Simulate phishing and train users on threat recognition.',
          icon: 'mdi-email-alert'
        }
      ]
    }
  },
  methods: {
    scrollToProducts() {
      const el = document.getElementById('products')
      if (el) el.scrollIntoView({ behavior: 'smooth' })
    }
  }
}
</script>

<style scoped>
.hero-section {
  background: linear-gradient(145deg, #1f3557, #2b4162);
  height: 100vh;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style> -->

<!-- <template>
  <v-container fluid class="pa-0">
    <section class="hero-section d-flex align-center justify-center">
      <v-container class="text-center">
        <h1 class="text-h2 mb-4 text-white" data-aos="fade-up">Cybersecurity Redefined</h1>
        <p class="text-white mb-6" data-aos="fade-in" data-aos-delay="200">Your digital shield against modern threats.</p>
        <v-btn
          color="primary"
          size="large"
          class="explore-btn"
          data-aos="zoom-in"
          data-aos-delay="400"
          @click="revealProduct"
        >
          Explore Now
        </v-btn>
      </v-container>
    </section>

    <transition name="slide-up">
      <section v-if="showProducts" class="product-section py-12">
        <v-container>
          <h2 class="text-center mb-10">Our Product Suite</h2>
          <v-row dense>
            <v-col
              v-for="product in products"
              :key="product.title"
              cols="12"
              md="4"
              class="mb-6"
            >
              <v-card class="pa-4 text-center" color="#1f3557" dark>
                <v-icon size="40" class="mb-3">{{ product.icon }}</v-icon>
                <h3 class="text-h6 mb-2">{{ product.title }}</h3>
                <p class="text-body-2 mb-3">{{ product.description }}</p>
                <v-btn color="primary" :to="product.route" variant="outlined">Learn More</v-btn>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </section>
    </transition>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      showProducts: false,
      products: [
        {
          title: 'Compliance Metrics',
          route: '/product/compliance-metrics',
          description: 'Track privacy KPIs, audits, data health, and regulatory status.',
          icon: 'mdi-chart-bar'
        },
        {
          title: 'Breach Management',
          route: '/product/breach-management',
          description: 'Detect, document, and act swiftly on data breaches.',
          icon: 'mdi-shield-alert'
        },
        {
          title: 'DPIA (Risk Assessment)',
          route: '/product/dpia',
          description: 'Assess and mitigate privacy risks across systems and vendors.',
          icon: 'mdi-clipboard-alert'
        },
        {
          title: 'Governance',
          route: '/product/governance',
          description: 'Centralize your privacy framework and organizational controls.',
          icon: 'mdi-account-group'
        },
        {
          title: 'DSR Management',
          route: '/product/dsr-management',
          description: 'Automate and fulfill Data Subject Requests efficiently.',
          icon: 'mdi-account-key'
        },
        {
          title: 'Vendor Management',
          route: '/product/vendor-management',
          description: 'Track and assess third-party compliance and contracts.',
          icon: 'mdi-truck'
        },
        {
          title: 'Phishing App',
          route: '/product/phishing-app',
          description: 'Simulate phishing and train users on threat recognition.',
          icon: 'mdi-email-alert'
        }
      ]
    };
  },
  methods: {
    revealProduct() {
      this.showProducts = true;
      // Optional: scroll to product section smoothly
      this.$nextTick(() => {
        const productEl = document.querySelector('.product-section');
        if (productEl) {
          productEl.scrollIntoView({ behavior: 'smooth' });
        }
      });
    }
  }
};
</script>

<style scoped>
.hero-section {
  height: 100vh;
  background: linear-gradient(145deg, #1f3557, #2b4162);
  color: white;
  position: relative;
  z-index: 1;
}

.product-section {
  background-color: #f4f7fa;
  position: relative;
  z-index: 2;
}

/* Slide-up animation */
.slide-up-enter-active {
  transition: all 0.6s ease;
}
.slide-up-leave-active {
  transition: all 0.4s ease;
}
.slide-up-enter-from {
  opacity: 0;
  transform: translateY(100%);
}
.slide-up-leave-to {
  opacity: 0;
  transform: translateY(100%);
}
</style> -->

<template>
  <v-container fluid class="pa-0">
    <!-- Hero Section -->
    <section class="hero-section d-flex align-center justify-center text-center">
      <div>
        <h1 class="text-h2 font-weight-bold mb-4" data-aos="fade-up">Cybersecurity Redefined</h1>
        <p class="text-subtitle-1 mb-6" data-aos="fade-in" data-aos-delay="200">
          Your digital shield against modern threats.
        </p>
        <v-btn
          color="primary"
          large
          data-aos="zoom-in"
          data-aos-delay="400"
          rounded="xl"
          @click="scrollToProducts"
        >
          Explore Now
        </v-btn>
      </div>
    </section>

    <!-- Product Overview Section -->
    <section
      v-if="showProducts"
      ref="productSection"
      class="product-section py-8 scroll-target"
    >
      <v-container>
        <h2 class="text-h4 text-center mb-8 font-weight-bold" data-aos="fade-up">
          Our Compliance Solutions
        </h2>
        <v-row dense>
          <v-col
            v-for="product in products"
            :key="product.title"
            cols="12"
            sm="6"
            md="6"
            class="mb-5"
            data-aos="zoom-in-up"
          >
            <v-card class="pa-4 text-center" color="#1f3557" dark>
              <v-icon size="40" class="mb-3">{{ product.icon }}</v-icon>
              <h3 class="text-h6 mb-2">{{ product.title }}</h3>
              <p class="text-body-2 mb-3">{{ product.description }}</p>
              <v-btn color="primary" :to="product.route" variant="outlined">
                Learn More
              </v-btn>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      showProducts: false,
      products: [
        {
          title: "Compliance Metrics",
          description: "Visualize KPIs, audit stats, consent records, and security performance.",
          route: "/product/compliance-metrics",
          icon: "mdi-chart-bar",
        },
        {
          title: "Breach Management",
          description: "Track, contain, and report incidents with real-time dashboards.",
          route: "/product/breach-management",
          icon: "mdi-shield-alert",
        },
        {
          title: "DPIA (Risk Assessment)",
          description: "Identify and mitigate risks through structured privacy assessments.",
          route: "/product/dpia",
          icon: "mdi-file-document-alert",
        },
        {
          title: "Governance",
          description: "Set rules and policies for better data handling and audit readiness.",
          route: "/product/governance",
          icon: "mdi-scale-balance",
        },
        {
          title: "DSR Management",
          description: "Handle data subject access and erasure requests seamlessly.",
          route: "/product/dsr-management",
          icon: "mdi-account-key",
        },
        {
          title: "Vendor Management",
          description: "Evaluate, onboard, and monitor vendors for compliance alignment.",
          route: "/product/vendor-management",
          icon: "mdi-briefcase-check",
        },
        {
          title: "Phishing App",
          description: "Run email simulations to train and track employee awareness.",
          route: "/product/phishing-app",
          icon: "mdi-email-alert",
        },
      ],
    };
  },
  methods: {
    scrollToProducts() {
      this.showProducts = true;
      this.$nextTick(() => {
        const el = this.$refs.productSection;
        if (el) {
          el.scrollIntoView({ behavior: "smooth" });
        }
      });
    },
  },
};
</script>

<style scoped>
.hero-section {
  min-height: 100vh;
  background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
  color: white;
  padding: 0 20px;
}

.product-section {
  background-color: #f5f5f5;
}

.scroll-target {
  scroll-margin-top: 80px;
}
</style>
