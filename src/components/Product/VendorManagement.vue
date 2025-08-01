<!-- <template>
  <v-container class="py-16">
    <h1 class="text-h3 font-weight-bold mb-4" data-aos="fade-up">Vendor Management</h1>
    <p class="text-body-1" data-aos="fade-up" data-aos-delay="100">
      Evaluate and monitor vendors’ data handling practices for compliance.
    </p>
  </v-container>
</template>

<script>
export default {
  name: 'VendorManagement'
}
</script> -->


<!-- <template>
  <v-container fluid class="vendor-page pa-0">
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Vendor Management</h1>
      <p class="text-subtitle-1">Monitor, assess, and manage third-party vendors handling sensitive data.</p>
    </div>

    <v-container class="mt-10" data-aos="fade-up">
      <v-row>
        <v-col cols="12" md="6">
          <h2 class="text-h5 font-weight-bold">Overview</h2>
          <p>
            Ensure your vendors comply with privacy and data protection standards by maintaining comprehensive records, performing risk assessments, and tracking data processing agreements (DPAs).
          </p>
        </v-col>
        <v-col cols="12" md="6">
          <v-img
            src="https://via.placeholder.com/500x300"
            alt="Vendor Management"
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
            <v-icon class="mb-2" size="32">{{ feature.icon }}</v-icon>
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
  name: "VendorManagement",
  data() {
    return {
      features: [
        {
          icon: "mdi-briefcase-account",
          title: "Vendor Registry",
          description: "Maintain an up-to-date inventory of all vendors and third parties."
        },
        {
          icon: "mdi-shield-check",
          title: "Compliance Checks",
          description: "Perform periodic compliance assessments and track certifications."
        },
        {
          icon: "mdi-file-document-multiple",
          title: "DPA Repository",
          description: "Store and manage Data Processing Agreements securely and accessibly."
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
.vendor-page {
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
  <v-container fluid class="vendor-page pa-0">
    <!-- Hero Section -->
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Vendor Management</h1>
      <p class="text-subtitle-1">
        Monitor, assess, and manage third-party vendors to ensure data protection and regulatory compliance.
      </p>
    </div>

    <!-- Overview Section -->
    <v-container class="mt-10" data-aos="fade-up">
      <v-row justify="center">
        <v-col cols="12" md="10">
          <h2 class="text-h5 font-weight-bold text-center mb-4">Overview</h2>
          <p class="text-body-1 text-center">
            The Vendor Management module ensures that third-party vendors or partners who process or access personal and sensitive data are held to the same data protection standards as your organization. It offers visibility into vendor risk, contract compliance, and data processing operations through audits, assessments, dashboards, and automated alerts.
          </p>
        </v-col>
      </v-row>
    </v-container>

    <!-- Key Features Section -->
    <v-container class="mt-12" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6 text-center">Key Features</h2>
      <v-row dense>
        <v-col cols="12" md="4" v-for="(feature, i) in features" :key="i" data-aos="zoom-in">
          <v-card class="pa-4 individual-feature-card" elevation="2">
            <v-icon size="36" class="mb-3" style="color: #90caf9">{{ feature.icon }}</v-icon>
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
  name: "VendorManagement",
  data() {
    return {
      features: [
        {
          title: "Vendor Register",
          description: "Maintain a registry of all third-party vendors with data access or processing roles.",
          icon: "mdi-clipboard-list-outline"
        },
        {
          title: "Risk Assessments",
          description: "Conduct and track periodic risk evaluations for each third-party vendor.",
          icon: "mdi-shield-search"
        },
        {
          title: "Contract Compliance",
          description: "Monitor data protection clauses and validity of contracts with vendors.",
          icon: "mdi-file-certificate-outline"
        },
        {
          title: "Visual Data Flow Mapping",
          description: "Map vendor data flows, data types handled, and processing locations.",
          icon: "mdi-vector-polyline"
        },
        {
          title: "Alerts & Notifications",
          description: "Get alerts on expiring contracts or overdue assessments automatically.",
          icon: "mdi-bell-ring-outline"
        },
        {
          title: "Audit Trail & Reports",
          description: "Log all vendor compliance activities and generate historical reports.",
          icon: "mdi-history"
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
.vendor-page {
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
