<script lang="ts" setup>
</script>

<template>
  <div class="container" id="mainContainer" style="display: none;">
    <div class="main-content">
      <aside class="sidebar">
        <ul class="sidebar-menu">
          <li>
            <a href="#" class="active" data-section="dashboard">
              <i class="fas fa-home"></i>
              <span>Dashboard</span>
            </a>
          </li>
          <li id="logoutItem">
            <a href="#" data-section="logout">
              <i class="fas fa-sign-out-alt"></i>
              <span>Logout</span>
            </a>
          </li>
        </ul>
      </aside>

      <main class="dashboard">
        <div class="section-header">
          <h2 class="section-title">My Passwords</h2>
          <button class="btn btn-primary" id="addPasswordBtn">
            <i class="fas fa-plus"></i>
            <span>Add Password</span>
          </button>
        </div>
        <div>
          <input type="text" id="searchInput" placeholder="Search passwords..." />
        </div>
        <div class="password-list" id="passwordList">
        </div>
      </main>
    </div>
  </div>

</template>