<!-- <template>
  <v-container class="py-16">
    <h1 class="text-h3 font-weight-bold mb-4" data-aos="fade-up">Incident Management</h1>
    <p class="text-body-1" data-aos="fade-up" data-aos-delay="100">
      Detect, track, and respond to privacy and security incidents.
    </p>
  </v-container>
</template>

<script>
export default {
  name: 'IncidentManagement'
}
</script> -->


<!-- <template>
  <v-container fluid class="py-12 px-4" style="background: linear-gradient(to bottom, #e3f0ff, #d0e0f5);">
    <v-row class="mb-12" align="center" justify="center">
      <v-col cols="12" md="8" class="text-center">
        <h1 class="display-1 font-weight-bold text-blue-darken-4" data-aos="fade-down">Breach Management</h1>
        <p class="subtitle-1 text-blue-grey-darken-1" data-aos="fade-up" data-aos-delay="200">
          Detect, contain, and respond to data breaches efficiently to minimize damage and ensure legal compliance.
        </p>
      </v-col>
    </v-row>

    <v-row class="mb-10" data-aos="fade-right">
      <v-col cols="12" md="10" class="mx-auto">
        <v-card flat class="pa-6" color="#ffffffaa" elevation="2" rounded="xl">
          <h2 class="text-h5 font-weight-medium mb-3">Overview</h2>
          <p>
            Our Breach Management module ensures swift incident response with built-in investigation tools, breach logging, containment support,
            and regulatory notification tracking. Centralize your breach handling process and reduce potential risks.
          </p>
        </v-card>
      </v-col>
    </v-row>

    <v-row data-aos="fade-up">
      <v-col cols="12">
        <h2 class="text-h5 text-center font-weight-bold mb-6 text-blue-grey-darken-2">Key Features</h2>
      </v-col>

      <v-col cols="12" md="4" v-for="(feature, index) in features" :key="index" data-aos="zoom-in" :data-aos-delay="index * 100">
        <v-card color="white" class="pa-5 text-center" rounded="lg" elevation="4">
          <v-icon color="primary" size="40">{{ feature.icon }}</v-icon>
          <h3 class="text-h6 font-weight-medium mt-3">{{ feature.title }}</h3>
          <p class="text-body-2 mt-2">{{ feature.description }}</p>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import AOS from 'aos'

export default {
  name: 'BreachManagement',
  data() {
    return {
      features: [
        {
          icon: 'mdi-alert-octagram',
          title: 'Breach Detection',
          description: 'Detect unusual activity and raise immediate alerts for potential breaches.'
        },
        {
          icon: 'mdi-security',
          title: 'Impact Assessment',
          description: 'Analyze the severity and scope of the breach to assess organizational impact.'
        },
        {
          icon: 'mdi-bell-alert',
          title: 'Regulatory Notification',
          description: 'Track deadlines and dispatch reports to relevant authorities like the DPA.'
        },
        {
          icon: 'mdi-timeline-check-outline',
          title: 'Incident Timeline',
          description: 'Maintain a timeline of breach events from detection to resolution.'
        },
        {
          icon: 'mdi-file-lock-outline',
          title: 'Containment Measures',
          description: 'Tools to help contain breaches and secure compromised data.'
        },
        {
          icon: 'mdi-chart-bar',
          title: 'Post-Breach Analysis',
          description: 'Learn from each incident with visual dashboards and root cause analytics.'
        }
      ]
    }
  },
  mounted() {
    AOS.init({ duration: 1000, once: true })
  }
}
</script>

<style scoped>
.text-blue-darken-4 {
  color: #0d47a1;
}
</style> -->


<!-- <template>
  <v-container fluid class="breach-management-page pa-0">
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Breach Management</h1>
      <p class="text-subtitle-1">Track and respond to data breaches with speed and accuracy.</p>
    </div>

    <v-container class="mt-10" data-aos="fade-up">
      <v-row>
        <v-col cols="12" md="6">
          <h2 class="text-h5 font-weight-bold">Overview</h2>
          <p>
            The Breach Management module provides tools to detect, manage, and report security breaches with audit trails and regulatory compliance.
          </p>
        </v-col>
        <v-col cols="12" md="6">
          <v-img
            src="https://via.placeholder.com/500x300"
            alt="Breach Management Dashboard"
            class="rounded"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mt-12" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6">Key Features</h2>
      <v-row dense>
        <v-col cols="12" md="4" v-for="(feature, index) in features" :key="index" data-aos="zoom-in" :data-aos-delay="index * 100">
          <v-card color="white" class="pa-5 text-center" rounded="lg" elevation="4">
            <v-icon color="primary" size="40">{{ feature.icon }}</v-icon>
            <h3 class="text-h6 font-weight-medium mt-3">{{ feature.title }}</h3>
            <p class="text-body-2 mt-2">{{ feature.description }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "BreachManagement",
  data() {
    return {
      features: [
        {
          icon: 'mdi-alert-octagram',
          title: 'Breach Detection',
          description: 'Detect unusual activity and raise immediate alerts for potential breaches.'
        },
        {
          icon: 'mdi-security',
          title: 'Impact Assessment',
          description: 'Analyze the severity and scope of the breach to assess organizational impact.'
        },
        {
          icon: 'mdi-bell-alert',
          title: 'Regulatory Notification',
          description: 'Track deadlines and dispatch reports to relevant authorities like the DPA.'
        },
        {
          icon: 'mdi-timeline-check-outline',
          title: 'Incident Timeline',
          description: 'Maintain a timeline of breach events from detection to resolution.'
        },
        {
          icon: 'mdi-file-lock-outline',
          title: 'Containment Measures',
          description: 'Tools to help contain breaches and secure compromised data.'
        },
        {
          icon: 'mdi-chart-bar',
          title: 'Post-Breach Analysis',
          description: 'Learn from each incident with visual dashboards and root cause analytics.'
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
.breach-management-page {
  background: linear-gradient(to bottom right, #f0f4f8, #e3f0ff);
  padding-bottom: 100px;
}

.hero-section {
  text-align: center;
  padding: 80px 20px;
  background-color: #1f3557;
  color: #e3f0ff;
}
</style>
 -->


<template>
  <v-container fluid class="breach-management-page pa-0">
    <!-- Hero Section -->
    <div class="hero-section" data-aos="fade-down">
      <h1 class="text-h2 text-primary mb-2">Breach Management</h1>
      <p class="text-subtitle-1">Track and respond to data breaches with speed and accuracy.</p>
    </div>

    <!-- Overview Section -->
    <v-container class="mt-10 text-center" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-4">Overview</h2>
      <v-row justify="center">
        <v-col cols="12" md="10">
          <p class="text-body-1">
            The Breach Management module is designed to streamline the entire lifecycle of a data breach — from detection to resolution. With a multi-step reporting wizard, automated severity classification, and SLA-based escalation, the system ensures rapid containment and compliance with global regulations like GDPR and DPDP.
            <br><br>
            Whether you’re reporting, investigating, or auditing, every step is logged with precision. Role-based access allows admins, handlers, compliance officers, and auditors to collaborate in real-time. Incident handlers can upload evidence, document RCA, and notify stakeholders, while templates help comply with regulatory disclosure timelines. The dashboard also provides live metrics on open breaches, SLA compliance, trends, and resolution timelines — all stored securely and retained for 5 years.
          </p>
        </v-col>
      </v-row>

      <!-- Image centered -->
      <v-row justify="center" class="mt-6">
        <v-col cols="12" md="8">
          <v-img
            src="https://via.placeholder.com/700x400"
            alt="Breach Management Dashboard"
            class="rounded mx-auto"
            max-width="100%"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>

    <!-- Features Section -->
    <v-container class="mt-12" data-aos="fade-up">
      <h2 class="text-h5 font-weight-bold mb-6 text-center">Key Features</h2>
      <v-row dense>
        <v-col
          cols="12"
          md="4"
          v-for="(feature, index) in features"
          :key="index"
          data-aos="zoom-in"
          :data-aos-delay="index * 100"
        >
          <v-card color="white" class="pa-5 text-center individual-feature-card" rounded="lg" elevation="4">
            <v-icon color="primary" size="40">{{ feature.icon }}</v-icon>
            <h3 class="text-h6 font-weight-medium mt-3">{{ feature.title }}</h3>
            <p class="text-body-2 mt-2">{{ feature.description }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "BreachManagement",
  data() {
    return {
      features: [
        {
          icon: 'mdi-form-select',
          title: 'Multi-Step Reporting',
          description: 'Submit breaches using a structured wizard: Incident, Systems, Impact, Evidence — with draft saving.'
        },
        {
          icon: 'mdi-auto-fix',
          title: 'Severity Classification',
          description: 'Automatically classify breaches by data type, individual count, and severity level.'
        },
        {
          icon: 'mdi-bell-alert-outline',
          title: 'Instant Alerts',
          description: 'Notify legal, compliance, and incident response teams immediately upon breach report.'
        },
        {
          icon: 'mdi-account-group',
          title: 'Role-Based Collaboration',
          description: 'Admins, Handlers, Compliance, and Auditors have tailored views and access privileges.'
        },
        {
          icon: 'mdi-message-text',
          title: 'Live Collaboration',
          description: 'Comment, upload files, and update logs simultaneously — all in real time.'
        },
        {
          icon: 'mdi-file-document-edit-outline',
          title: 'Pre-Filled Authority Notices',
          description: 'Auto-generate DPA notification templates per jurisdiction (GDPR, DPDP, etc.).'
        },
        {
          icon: 'mdi-chart-box-outline',
          title: 'Breach Metrics Dashboard',
          description: 'Real-time stats for active breaches, SLA compliance, and root cause breakdowns.'
        },
        {
          icon: 'mdi-folder-key-outline',
          title: 'Secure Archiving',
          description: 'Retain breaches for 5 years and then archive securely with integrity validation.'
        },
        {
          icon: 'mdi-history',
          title: 'Full Audit Trails',
          description: 'Track every user action with timestamps, justification, and digital signatures.'
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
.breach-management-page {
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
