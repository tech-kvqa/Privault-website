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
export default {
  name: "ComplianceMetrics",
  data() {
    return {
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
  },
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


</style>
