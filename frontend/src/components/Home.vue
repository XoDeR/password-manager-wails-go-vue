<script lang="ts" setup>
import { ref, onMounted } from 'vue';
import PasswordManager from './PasswordManager.vue';
import Auth from './Auth.vue';

const isAuthenticated = ref(false);

////
const handleLoginSuccess = () => {
  sessionStorage.setItem('vaultpass_authenticated', 'true');
  isAuthenticated.value = true;
};
////

onMounted(() => {
  const authStatus = sessionStorage.getItem('vaultpass_authenticated');
  isAuthenticated.value = authStatus === 'true';
});
</script>

<template>
  <PasswordManager v-if="isAuthenticated" />
  <Auth v-else @login-success="handleLoginSuccess" />
</template>