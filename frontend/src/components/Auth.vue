<script lang="ts" setup>
</script>

<template>
  <div class="container" id="authContainer">
    <div class="auth-card">
      <div class="auth-tabs">
        <button class="auth-tab active" id="loginTab">Login</button>
        <button class="auth-tab" id="registerTab">Register</button>
      </div>
      <div class="auth-form-container">
        <LoginForm />
        <RegisterForm />
      </div>
    </div>
  </div>
</template>

<style>
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  border-radius: var(--border-radius);
  font-weight: 500;
  cursor: pointer;
  transition: var(--transition);
  border: none;
}

.btn-primary {
  background-color: var(--primary-color);
  color: white;
}

.btn-primary:hover {
  background-color: #4338ca;
}

.btn-outline {
  background-color: transparent;
  color: white;
  border: 1px solid white;
}

.btn-outline:hover {
  background-color: rgba(255, 255, 255, 0.1);
}
</style>