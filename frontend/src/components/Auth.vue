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
        <!-- Login Form -->
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

        <!-- Register Form -->
        <form id="registerForm" class="auth-form" style="display: none;">
          <div class="form-group">
            <label for="registerPassword">Create Password</label>
            <div style="position: relative;">
              <input type="password" id="registerPassword" class="form-control" required style="padding-right: 40px;">
              <button type="button" id="registerTogglePassword" class="btn btn-outline"
                style="position: absolute; right: 5px; top: 50%; transform: translateY(-50%); color: var(--dark-color); border: none; background: none; padding: 5px;">
                <i class="fas fa-eye"></i>
              </button>
            </div>
          </div>
          <div class="form-group">
            <label for="confirmPassword">Confirm Password</label>
            <div style="position: relative;">
              <input type="password" id="confirmPassword" class="form-control" required style="padding-right: 40px;">
              <button type="button" id="confirmTogglePassword" class="btn btn-outline"
                style="position: absolute; right: 5px; top: 50%; transform: translateY(-50%); color: var(--dark-color); border: none; background: none; padding: 5px;">
                <i class="fas fa-eye"></i>
              </button>
            </div>
          </div>
          <div class="form-group">
            <label for="encryptDb">Would you like to store your data more securely? <br><span style="color: #cc0000;">⚠️
                Forgotten password cannot be recovered.</span></label>

            <select id="encryptDb" class="form-control" required>
              <option value="" disabled selected>Select an option</option>
              <option value="yes">Yes</option>
              <option value="no">No</option>
            </select>
          </div>
          <div class="form-actions">
            <button type="submit" class="btn btn-primary btn-block">Register</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>