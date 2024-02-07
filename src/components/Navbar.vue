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
            <div class="navbar-item">Toggle</div>
          </div>
        </div>
      </div>
      <div class="nav-end">
        <p>Malibu, California, USA</p>
        <p class="end-text">Hotel June Malibu</p>
        <p>Seaside Retreat in Malibu</p>
      </div>
    </nav>
  </template>
  
  <script setup>
  // No script logic is currently active
  </script>
  
  <style scoped>
  .navbar {
    background: linear-gradient(rgb(0,0, 0, .5), rgba(0, 0, 0, 0.5)), url('../assets/Banner.png');
    border-radius: 0 0 32px 32px;
    background-size: cover;
    background-position: center ;
    height: 423px;
    width: 1440px;
    margin: auto;
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
    height: 27px; /* Fix typo: add "px" to height */
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
  }
  </style>
  