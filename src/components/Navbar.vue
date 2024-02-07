<template>
  <nav class="navbar">
    <div class="navbar-top">
      <div class="navbar-links">
        <div class="navbar-left">
          HOLIGAY
        </div>
        <div class="navbar-right">
          <div class="navbar-item">My Account</div>
          <div class="navbar-item">Guide</div>
          <div class="navbar-item">USD</div>
          <div class="navbar-item toggle-btn" @click="toggleMenu">

            <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M0.833984 4.16666H19.1673M0.833984 9.99999H19.1673M0.833984 15.8333H19.1673" stroke="white"
                stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>

          </div>
        </div>
      </div>
    </div>
    <div class="nav-end">
      <p>Malibu, California, USA</p>
      <p class="end-text">Hotel June Malibu</p>
      <p>Seaside Retreat in Malibu</p>
    </div>
    <!-- Add mobile menu -->
    <div class="mobile-menu" :class="{ 'show-menu': isMenuOpen }">
      <div class="navbar-item">My Account</div>
      <div class="navbar-item">Guide</div>
      <div class="navbar-item">USD</div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value;
}
</script>

<style scoped>
.navbar {
  background: linear-gradient(rgb(0, 0, 0, .5), rgba(0, 0, 0, 0.5)), url('../assets/Banner.png');
  border-radius: 0 0 32px 32px;
  background-size: cover;
  background-position: center;
  height: 423px;
  max-width: 1440px;
  margin: auto;
}

/* Responsive Styles */
@media screen and (max-width: 960px) {
  .navbar-item {
    display: none;
  }

  .toggle-btn {
    display: block;
    /* Show toggle button for smaller screens */
  }

  .mobile-menu {
    display: none;
    /* Hide mobile menu by default */
    background-color: #333;
    padding: 20px;
    position: absolute;
    top: 67px;
    left: 0;
    right: 0;
  }

  .show-menu {
    display: flex;
    /* Show mobile menu when active */
    flex-direction: column;
    align-items: center;
  }
}

.navbar-top {
  height: 67px;
  align-items: center;
}

.navbar-links {
  color: #fff;
  padding: 10px;
  display: flex;
  justify-content: space-between;
}

.navbar-left {
  width: 131px;
  height: 27px;
  /* Fix typo: add "px" to height */
  font-size: 30px;
  font-weight: 400;
}

.navbar-right {
  display: flex;
  margin-top: 2px;
}

.navbar-item {
  margin: 0 10px;
}

.toggle-btn {
  background-color: transparent;
  color: #fff;
  border: none;
  cursor: pointer;
}

.nav-end {
  text-align: center;
  height: 171px;
  padding-top: 50px;
}

.end-text {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 600;
  font-size: 64px;
  letter-spacing: -2px;
  color: white;
  margin: 20px;
}</style>
