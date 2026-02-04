<template>
  <form id="loginForm" class="auth-form">
    <div class="form-group">
      <label for="loginPassword">Password</label>
      <div style="position: relative;">
        <input type="password" id="loginPassword" class="form-control" required style="padding-right: 40px;">
        <button type="button" id="loginTogglePassword" class="btn btn-outline"
          style="position: absolute; right: 5px; top: 50%; transform: translateY(-50%); color: var(--dark-color); border: none; background: none; padding: 5px;">
          <i class="fas fa-eye"></i>
        </button>
      </div>
    </div>
    <div class="form-actions">
      <button type="submit" class="btn btn-primary btn-block">Login</button>
    </div>
  </form>
</template>