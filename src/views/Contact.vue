<!-- <template>
  <v-container>
    <h2>Contact Us</h2>
    <v-form>
      <v-text-field label="Name" required></v-text-field>
      <v-text-field label="Email" required></v-text-field>
      <v-textarea label="Message" required></v-textarea>
      <v-btn color="primary" type="submit">Send</v-btn>
    </v-form>
  </v-container>
</template> -->


<!-- <template>
  <v-container class="py-12">
    <v-row justify="center">
      <v-col cols="12" md="8" lg="6">
        <h2 class="text-h4 font-weight-bold mb-6 text-center">Contact Us</h2>

        <v-card elevation="4" class="pa-6 rounded-xl">
          <v-form @submit.prevent="submitForm" ref="contactForm" v-model="formValid">
            <v-text-field
              label="Name"
              v-model="form.name"
              :rules="[v => !!v || 'Name is required']"
              required
              outlined
              dense
              class="mb-4"
            />

            <v-text-field
              label="Email"
              v-model="form.email"
              :rules="[v => !!v || 'Email is required', v => /.+@.+\..+/.test(v) || 'Enter a valid email']"
              required
              outlined
              dense
              class="mb-4"
            />

            <v-textarea
              label="Message"
              v-model="form.message"
              :rules="[v => !!v || 'Message is required']"
              required
              outlined
              rows="4"
              class="mb-6"
            />

            <v-btn color="primary" type="submit" :disabled="!formValid" block>
              Send Message
            </v-btn>
          </v-form>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: '',
      },
      formValid: false,
    };
  },
  methods: {
    submitForm() {
      if (this.$refs.contactForm.validate()) {
        // You can replace this with actual API call
        console.log('Form submitted:', this.form);

        // Reset form
        this.form = { name: '', email: '', message: '' };
        this.$refs.contactForm.resetValidation();
      }
    },
  },
};
</script>

<style scoped>
h2 {
  color: #e3f0ff;
}
</style> -->


<template>
  <v-container fluid class="contact-section py-12">
    <v-row justify="center" align="center">
      <v-col cols="12" md="10">
        <v-card class="pa-8 rounded-xl" elevation="8">
          <v-row>
            <!-- LEFT: Contact Info -->
            <v-col cols="12" md="5" class="pe-md-8 mb-6 mb-md-0 border-md-e">
              <h2 class="text-h5 font-weight-bold mb-4">Get in Touch</h2>
              <p class="text-body-2 mb-6">
                We'd love to hear from you! Whether you have a question about features, pricing, or anything else, our team is ready to answer.
              </p>
              <div class="mb-4">
                <v-icon color="primary" class="me-3">mdi-email</v-icon>
                <span></span>
              </div>
              <div class="mb-4">
                <v-icon color="primary" class="me-3">mdi-phone</v-icon>
                <span></span>
              </div>
              <div class="mb-4">
                <v-icon color="primary" class="me-3">mdi-map-marker</v-icon>
                <span>202, DLF GALLERIA MALL, MAYUR VIHAR, PHASE-1, DELHI-110091, INDIA</span>
              </div>
            </v-col>

            <!-- RIGHT: Form -->
            <v-col cols="12" md="7">
              <h2 class="text-h5 font-weight-bold mb-4">Contact Form</h2>
              <v-form @submit.prevent="submitForm" ref="contactForm" v-model="formValid">
                <v-text-field
                  v-model="form.name"
                  label="Name"
                  :rules="[v => !!v || 'Name is required']"
                  outlined
                  dense
                  class="mb-4"
                />
                <v-text-field
                  v-model="form.email"
                  label="Email"
                  :rules="[
                    v => !!v || 'Email is required',
                    v => /.+@.+\..+/.test(v) || 'Enter a valid email'
                  ]"
                  outlined
                  dense
                  class="mb-4"
                />
                <v-textarea
                  v-model="form.message"
                  label="Message"
                  :rules="[v => !!v || 'Message is required']"
                  outlined
                  rows="4"
                  class="mb-6"
                />
                <v-btn color="primary" type="submit" :disabled="!formValid" block>
                  Send Message
                </v-btn>
              </v-form>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: '',
      },
      formValid: false,
    };
  },
  methods: {
    submitForm() {
      if (this.$refs.contactForm.validate()) {
        console.log('Form submitted:', this.form);
        this.form = { name: '', email: '', message: '' };
        this.$refs.contactForm.resetValidation();
      }
    },
  },
};
</script>

<style scoped>
.contact-section {
  background: linear-gradient(to right, #f4f8ff, #e6f0ff);
}

.v-card {
  background-color: white;
  border-radius: 16px;
}

.border-md-e {
  border-right: 1px solid #eee;
}
</style>
