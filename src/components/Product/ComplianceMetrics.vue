<!-- <template>
  <v-container class="py-16">
    <h1 class="text-h3 font-weight-bold mb-4" data-aos="fade-up">Compliance Metrics</h1>
    <p class="text-body-1" data-aos="fade-up" data-aos-delay="100">
      View real-time metrics for your compliance readiness and data privacy efforts.
    </p>
  </v-container>
</template>

<script>
export default {
  name: 'ComplianceMetrics'
}
</script> -->


<!-- <template>
  <v-container fluid class="compliance-metrics-page pa-0">
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Compliance Metrics</h1>
      <p class="text-subtitle-1">Track and visualize your organization's compliance health in real-time.</p>
    </div>

    <v-container class="mt-10" data-aos="fade-up">
      <v-row>
        <v-col cols="12" md="6">
          <h2 class="text-h5 font-weight-bold">Overview</h2>
          <p>
            The Compliance Metrics module provides real-time dashboards, alerts, and insights to ensure adherence to data protection regulations.
          </p>
        </v-col>
        <v-col cols="12" md="6">
          <v-img
            src="https://via.placeholder.com/500x300"
            alt="Compliance Metrics Dashboard"
            class="rounded"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mt-12" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Key Features</h2>
      <v-row dense>
        <v-col cols="12" md="4" v-for="(feature, i) in features" :key="i" data-aos="zoom-in">
          <v-card class="pa-4" elevation="2">
            <h3 class="text-subtitle-1 font-weight-medium">{{ feature.title }}</h3>
            <p class="text-body-2">{{ feature.description }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "ComplianceMetrics",
  data() {
    return {
      features: [
        {
          title: "Real-Time Dashboard",
          description: "Visualize compliance scores and regulatory KPIs in real time."
        },
        {
          title: "Automated Alerts",
          description: "Receive alerts for non-compliance incidents or threshold breaches."
        },
        {
          title: "Historical Reports",
          description: "Generate and export compliance trend reports across time periods."
        }
      ]
    };
  },
  mounted() {
    import("aos/dist/aos.css");
    import("aos").then(AOS => AOS.init({ duration: 1000 }));
  }
};
</script>

<style scoped>
.compliance-metrics-page {
  background: linear-gradient(to bottom right, #f0f4f8, #e3f0ff);
  padding-bottom: 100px;
}

.hero-section {
  text-align: center;
  padding: 80px 20px;
  background-color: #1f3557;
  color: #e3f0ff;
}
</style> -->

<template>
  <v-container fluid class="compliance-metrics-page pa-0">
    <!-- Hero Section -->
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Compliance Metrics</h1>
      <p class="text-subtitle-1">
        Track and visualize your organization's compliance health in real-time.
      </p>
    </div>

    <!-- Overview Section -->
    <!-- <v-container class="mt-10" data-aos="fade-up">
      <v-row>
        <v-col cols="12" md="6">
          <h2 class="text-h5 font-weight-bold">Overview</h2>
          <p>
            Our Compliance Metrics suite centralizes your privacy governance capabilities. Monitor and manage privacy policy generation, cross-border data transfers, and jurisdictional compliance from one intelligent interface.
            Automate document creation, assess international transfer risks, and stay aligned with evolving global laws like GDPR, PDPA, CCPA, and more.
            The platform enables real-time visibility into data flow, generates audit-ready documentation, and integrates with other modules such as Consent and Vendor Management — offering a comprehensive, always-current compliance picture.
          </p>
        </v-col>
        <v-col cols="12" md="6">
          <v-img
            src="https://via.placeholder.com/500x300"
            alt="Compliance Metrics Dashboard"
            class="rounded"
          ></v-img>
        </v-col>
      </v-row>
    </v-container> -->

    <!-- Overview Section -->
    <v-container class="mt-10 text-center" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-4">Overview</h2>

      <!-- Full-width intro paragraph, centered text -->
      <v-row justify="center">
        <v-col cols="12" md="10">
          <p class="text-body-1">
            Our Compliance Metrics suite centralizes your privacy governance capabilities. Monitor and manage privacy policy generation, cross-border data transfers, and jurisdictional compliance from one intelligent interface.
            Automate document creation, assess international transfer risks, and stay aligned with evolving global laws like GDPR, PDPA, CCPA, and more.
            The platform enables real-time visibility into data flow, generates audit-ready documentation, and integrates with other modules such as Consent and Vendor Management — offering a comprehensive, always-current compliance picture.
          </p>
        </v-col>
      </v-row>

      <!-- Centered image below -->
      <v-row justify="center" class="mt-6">
        <v-col cols="12" md="8">
          <v-img
            src="https://via.placeholder.com/700x400"
            alt="Compliance Metrics Dashboard"
            class="rounded mx-auto"
            max-width="100%"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>

    <v-divider class="border-opacity-100" color="success"></v-divider>

    <!-- Screenshots Section -->
    <!-- <v-container class="mt-12 screenshots-section text-center" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Product Screenshots</h2>
      <div class="screenshot-gallery">
        <img :src="image1" alt="Dashboard" class="screenshot-img img1" />
        <img :src="image2" alt="Reports" class="screenshot-img img2" />
        <img :src="image3" alt="Trends" class="screenshot-img img3" />
        <img :src="image4" alt="Trends" class="screenshot-img img4" />
      </div>
    </v-container> -->

    <!-- Screenshots Section -->
    <!-- <v-container class="mt-12 screenshots-section text-center" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Product Screenshots</h2>
      
      <div class="screenshot-gallery">
        <img 
          v-for="(img, index) in images" 
          :key="index" 
          :src="img" 
          :class="['screenshot-img', { active: index === activeIndex }]" 
          alt="Screenshot"
        />
      </div>
    </v-container> -->

    <!-- Screenshots Section -->
    <v-container class="mt-12 screenshots-section text-center" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Product Screenshots</h2>
      <v-carousel
        v-model="activeIndex"
        cycle
        hide-delimiters
        height="380"
        max-width="800"
        interval="4000"
        class="peek-carousel"
        show-arrows="hover"
      >
        <v-carousel-item
          v-for="(img, index) in images"
          :key="index"
          class="peek-slide"
          :class="{
            active: index === activeIndex,
            prev: index === (activeIndex - 1 + images.length) % images.length,
            next: index === (activeIndex + 1) % images.length
          }"
          @click="goToSlide(index)"
        >
          <v-img
            :src="img"
            class="screenshot-img"
          />
        </v-carousel-item>
      </v-carousel>
    </v-container>

    <v-divider class="border-opacity-100" color="success"></v-divider>

    <!-- Features Section -->
    <v-container class="mt-12" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Key Features</h2>
      <v-row dense>
        <v-col cols="12" md="4" v-for="(feature, i) in features" :key="i" data-aos="zoom-in">
          <v-card class="pa-4 individual-feature-card" elevation="2">
            <v-icon size="32" color="primary" class="mb-2">{{ feature.icon }}</v-icon>
            <h3 class="text-subtitle-1 font-weight-medium">{{ feature.title }}</h3>
            <p class="text-body-2">{{ feature.description }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
import image1 from "@/assets/edited/Complinace/compliance report.png"
import image2 from "@/assets/edited/Complinace/cross border dashboard.png"
import image3 from "@/assets/edited/Complinace/privacy policy report.png"
import image4 from "@/assets/edited/Complinace/privacy_policy questionnaire.png"
export default {
  name: "ComplianceMetrics",
  data() {
    return {
      // image1,
      // image2,
      // image3,
      // image4,
      activeIndex: 0,
      slideInterval: null,
      images: [
        require("@/assets/edited/Complinace/compliance report.png"),
        require("@/assets/edited/Complinace/cross border dashboard.png"),
        require("@/assets/edited/Complinace/privacy policy report.png"),
        require("@/assets/edited/Complinace/privacy_policy questionnaire.png")
      ],
      features: [
        {
          title: "Cross-Border Mapping",
          icon: "mdi-earth",
          description: "Identify source and destination countries, legal mechanisms, and transfer volume trends.",
        },
        {
          title: "SCC & BCR Management",
          icon: "mdi-file-lock",
          description: "Upload SCCs/BCRs, set expiry alerts, and maintain immutable audit trails for transfers.",
        },
        {
          title: "Transfer Risk Analysis",
          icon: "mdi-shield-alert",
          description: "Assess risk levels based on predefined criteria and highlight non-compliant jurisdictions.",
        },
        {
          title: "Privacy Policy Generator",
          icon: "mdi-file-document-edit",
          description: "Generate, edit, and version privacy policies based on jurisdiction-specific checklists.",
        },
        {
          title: "Policy Compliance Checker",
          icon: "mdi-check-decagram",
          description: "Compare existing policies against legal frameworks and generate gap analysis reports.",
        },
        {
          title: "Multi-Jurisdiction Support",
          icon: "mdi-gavel",
          description: "Ensure compliance across GDPR, PDPA, LGPD, CCPA and more from one unified interface.",
        },
      ],
    };
  },
  mounted() {
    import("aos/dist/aos.css");
    import("aos").then((AOS) => AOS.init({ duration: 1000, once: true }));

    // Auto-slide every 3s
    this.slideInterval = setInterval(() => {
      this.activeIndex = (this.activeIndex + 1) % this.images.length;
    }, 3000);
  },

  methods: {
    goToSlide(index) {
      this.activeIndex = index;
    }
  }
};
</script>

<style scoped>
.compliance-metrics-page {
  background: linear-gradient(to bottom right, #f0f4f8, #e3f0ff);
  padding-bottom: 100px;
}

.hero-section {
  text-align: center;
  padding: 80px 20px;
  background-color: #1f3557;
  color: #e3f0ff;
}

.individual-feature-card {
  transition: all 0.3s ease;
  transform: scale(1);
  z-index: 1;
  position: relative;
}

.individual-feature-card:hover {
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.2);
  z-index: 10;
  background-color: #e3f0ff; /* Light blue-gray */
  color: #1f3557; /* Text color */
}

.individual-feature-card:hover h3,
.individual-feature-card:hover p,
.individual-feature-card:hover .v-icon {
  color: #1f3557 !important;
}

/* .screenshot-gallery {
  position: relative;
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
  height: 500px;
} */

/* .screenshot-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
} */

/* .screenshot-gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: auto;
  gap: 20px;
  justify-items: center;
  align-items: start;
} */

/* latest style code. Before is correct. */

/* Style 1 */

/* .screenshot-gallery {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-auto-rows: 200px;
  gap: 20px;
  justify-items: center;
  align-items: center;
}

.screenshot-gallery img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  z-index: 1;
}

.img1 { grid-column: span 3; grid-row: span 2; }
.img2 { grid-column: span 3; grid-row: span 1; }
.img3 { grid-column: span 2; grid-row: span 1; }
.img4 { grid-column: span 4; grid-row: span 1; }

.screenshot-gallery img:hover {
  width: 600px;
  height: auto;
  transform: rotate(var(--angle));
  z-index: 10;
  box-shadow: 0 12px 30px rgba(0,0,0,0.35);
  animation: none
} */

/* Style 2 */


/* .screenshot-gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  max-width: 900px;
  margin: 0 auto;
}

.screenshot-gallery img {
  width: 300px;
  height: 200px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  transition: all 0.4s ease;
  cursor: pointer;
}

.screenshot-gallery img:hover {
  width: 500px;
  height: 350px;
  object-fit: contain;
  z-index: 10;
  box-shadow: 0 12px 30px rgba(0,0,0,0.35);
  background: #fff;
} */

/* Style 3 */

/* .screenshot-gallery {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  overflow: visible;
  max-width: 1000px;
  margin: 0 auto;
  position: relative;
}

.screenshot-gallery img {
  width: 250px;
  height: 160px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  transition: all 0.6s ease;
  opacity: 0.6;
  z-index: 1;
  cursor: pointer;
}

.screenshot-gallery img.active {
  width: 400px;
  height: 260px;
  object-fit: contain;
  opacity: 1;
  z-index: 2;
  background: #fff;
  padding: 5px;
}

.screenshot-gallery img:hover {
  transform: scale(1.2);
  z-index: 3;
  box-shadow: 0 12px 30px rgba(0,0,0,0.35);
}


@keyframes float {
  0% { transform: translateY(0px) rotate(var(--angle)); }
  50% { transform: translateY(-10px) rotate(var(--angle)); }
  100% { transform: translateY(0px) rotate(var(--angle)); }
} */

/* Style 4 */

.peek-carousel {
  overflow: visible !important;
  position: relative;
}

.peek-slide {
  display: block !important;
  position: absolute !important;
  top: 0;
  left: 50%;
  width: 600px;
  height: 350px;
  transition: all 0.6s ease;
  opacity: 0;
  transform: translateX(-50%) scale(0.8);
  z-index: 1;
  pointer-events: none;
}


.peek-slide.active {
  opacity: 1;
  transform: translateX(-50%) scale(1);
  z-index: 3;
  pointer-events: auto;
}

.peek-slide.prev {
  opacity: 0.7;
  transform: translateX(-170%) scale(0.9);
  z-index: 2;
  pointer-events: auto;
  cursor: pointer;
}

.peek-slide.next {
  opacity: 0.7;
  transform: translateX(70%) scale(0.9);
  z-index: 2;
  pointer-events: auto;
  cursor: pointer;
}


.screenshot-img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  border-radius: 16px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  transition: transform 0.4s ease, box-shadow 0.4s ease;
}


.peek-slide.active:hover {
  width: 650px !important;
  height: 400px !important;
  z-index: 5;
}

</style>
