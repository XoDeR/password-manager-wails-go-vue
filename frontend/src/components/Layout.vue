<script lang="ts" setup>
</script>

<template>
  <header>
    <div class="container header-content">
      <div class="logo">
        <i class="fas fa-lock"></i>
        <span>Password Vault</span>
      </div>
    </div>
  </header>
</template>

<style>
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem;
}

header {
  background-color: var(--primary-color);
  color: white;
  padding: 1rem 0;
  box-shadow: var(--shadow-md);
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 1.5rem;
  font-weight: 600;
}

.logo i {
  font-size: 1.75rem;
}
</style>
