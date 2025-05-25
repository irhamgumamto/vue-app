<template>
  <v-container class="d-flex justify-center align-center" style="min-height: 100vh;">
    <v-card elevation="8" class="pa-6" max-width="400">
      <h2 class="text-center mb-6">Login</h2>
      <h1 class="text-center mb-6">Silahkan Login Terlebih Dahulu</h1>

      <v-form @submit.prevent="handleLogin">
        <v-text-field
          v-model="email"
          label="Email"
          type="email"
          required
        ></v-text-field>

        <v-text-field
          v-model="password"
          label="Password"
          type="password"
          required
        ></v-text-field>

        <v-btn type="submit" color="primary" block>Login</v-btn>
      </v-form>

      <div class="text-danger mt-3" v-if="error">
        {{ error }}
      </div>
    </v-card>
  </v-container>
</template>

<script setup>
import { ref } from 'vue'
import { useRouter } from 'vue-router'

const email = ref('')
const password = ref('')
const error = ref('')
const router = useRouter()

const handleLogin = () => {
  // Simulasi login, kamu bisa ganti dengan API login asli
  if (email.value === 'admin@example.com' && password.value === 'password') {
    error.value = ''
    router.push('/') // Redirect ke home
  } else {
    error.value = 'Email atau password salah'
  }
}
</script>
