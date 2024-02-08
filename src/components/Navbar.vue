<template>
  <div class="navbar">
    <nav>
      <ul class="sidebar">
        <li @click="toggleHide"><a href="#"><svg xmlns="http://www.w3.org/2000/svg" fill="white" height="24"
              viewBox="0 -960 960 960" width="24">
              <path
                d="m256-200-56-56 224-224-224-224 56-56 224 224 224-224 56 56-224 224 224 224-56 56-224-224-224 224Z" />
            </svg></a></li>
        <li><a href="#">My Account</a></li>
        <li><a href="#">Guide</a></li>
        <li><a href="#">USD</a></li>
      </ul>


      <ul>
        <li class="hideOnMobile"><a href="#">
            <img style="width: 131px; height: 27px;" src="../assets/holigay.png" alt="">
          </a></li>
        <li class="hideOnMobile"><a href="#">My Account</a></li>
        <li class="hideOnMobile"><a href="#">Guide</a></li>
        <li class="hideOnMobile"><a href="#">
            <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M9 15.75C10.4962 15.7499 11.9501 15.2529 13.1333 14.337C14.3164 13.4211 15.1619 12.1382 15.537 10.6898M9 15.75C7.50376 15.7499 6.04991 15.2529 4.86673 14.337C3.68356 13.4211 2.83806 12.1382 2.463 10.6898M9 15.75C10.8638 15.75 12.375 12.7275 12.375 9C12.375 5.2725 10.8638 2.25 9 2.25M9 15.75C7.13625 15.75 5.625 12.7275 5.625 9C5.625 5.2725 7.13625 2.25 9 2.25M15.537 10.6898C15.6758 10.1498 15.75 9.5835 15.75 9C15.7519 7.83908 15.4529 6.69749 14.8823 5.6865M15.537 10.6898C13.5369 11.7985 11.2869 12.3786 9 12.375C6.6285 12.375 4.40025 11.7638 2.463 10.6898M2.463 10.6898C2.32106 10.1377 2.2495 9.56998 2.25 9C2.25 7.79625 2.565 6.66525 3.11775 5.6865M9 2.25C10.1972 2.2495 11.3729 2.56752 12.4066 3.17142C13.4403 3.77533 14.2948 4.64338 14.8823 5.6865M9 2.25C7.80282 2.2495 6.62706 2.56752 5.59336 3.17142C4.55966 3.77533 3.70523 4.64338 3.11775 5.6865M14.8823 5.6865C13.2493 7.10095 11.1604 7.87811 9 7.875C6.7515 7.875 4.695 7.05 3.11775 5.6865"
                stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>

            USD</a>
        </li>
        <li class="hideOnMobile"><a href="#">
            <svg width="49" height="24" viewBox="0 0 49 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect width="49" height="24" rx="12" fill="#5358FF" />
              <circle cx="12" cy="12" r="10" fill="white" />
              <path
                d="M35 4.5V6.375M40.3033 6.69667L38.9775 8.0225M42.5 12H40.625M40.3033 17.3033L38.9775 15.9775M35 17.625V19.5M31.0225 15.9775L29.6967 17.3033M29.375 12H27.5M31.0225 8.0225L29.6967 6.69667M38.125 12C38.125 12.8288 37.7958 13.6237 37.2097 14.2097C36.6237 14.7958 35.8288 15.125 35 15.125C34.1712 15.125 33.3763 14.7958 32.7903 14.2097C32.2042 13.6237 31.875 12.8288 31.875 12C31.875 11.1712 32.2042 10.3763 32.7903 9.79029C33.3763 9.20424 34.1712 8.875 35 8.875C35.8288 8.875 36.6237 9.20424 37.2097 9.79029C37.7958 10.3763 38.125 11.1712 38.125 12Z"
                stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>

          </a>
        </li>
        <li class="menu-button" style="margin-right: auto;"><a href="">
            <svg width="10" height="18" viewBox="0 0 10 18" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M8.75 16.5L1.25 9L8.75 1.5" stroke="white" stroke-width="1.5" stroke-linecap="round"
                stroke-linejoin="round" />
            </svg>

          </a></li>
        <li class="menu-button" style="margin-right: auto;"><a href=""><img style="width: 88px; height: 18px;"
              src="../assets/holigay.png" alt=""></a></li>
        <li class="menu-button" @click="toggleOpen">

          <a href="#"><svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M0.833984 4.16666H19.1673M0.833984 9.99999H19.1673M0.833984 15.8333H19.1673" stroke="white"
                stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>
          </a>
        </li>
      </ul>


    </nav>
    <div class="nav-end">
      <div class="nav-end-text">
        <svg width="21" height="21" viewBox="0 0 21 21" fill="none" xmlns="http://www.w3.org/2000/svg">
          <g opacity="0.4">
            <path
              d="M13 9.25C13 9.91304 12.7366 10.5489 12.2678 11.0178C11.7989 11.4866 11.163 11.75 10.5 11.75C9.83696 11.75 9.20107 11.4866 8.73223 11.0178C8.26339 10.5489 8 9.91304 8 9.25C8 8.58696 8.26339 7.95107 8.73223 7.48223C9.20107 7.01339 9.83696 6.75 10.5 6.75C11.163 6.75 11.7989 7.01339 12.2678 7.48223C12.7366 7.95107 13 8.58696 13 9.25Z"
              stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            <path
              d="M16.75 9.25C16.75 15.2017 10.5 18.625 10.5 18.625C10.5 18.625 4.25 15.2017 4.25 9.25C4.25 7.5924 4.90848 6.00268 6.08058 4.83058C7.25268 3.65848 8.8424 3 10.5 3C12.1576 3 13.7473 3.65848 14.9194 4.83058C16.0915 6.00268 16.75 7.5924 16.75 9.25Z"
              stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
          </g>
        </svg>
        <p>Malibu, California, USA</p>
      </div>
      <p class="end-text">Hotel June Malibu</p>
      <p class="nav-end-text">Seaside Retreat in Malibu</p>
    </div>

  </div>
</template>

<script setup>

function toggleOpen() {
  const sidebar = document.querySelector(".sidebar")
  sidebar.style.display = 'flex'
}

function toggleHide() {
  const sidebar = document.querySelector(".sidebar")
  sidebar.style.display = 'none'
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

.sidebar {
  display: none;
  background-color: #6c6b6b;
  padding: 20px;
  position: fixed;
  top: 0;
  right: 0px;
  height: 100vh;
  width: 300px;
  z-index: 2;
  display: none;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  text-decoration: none;
  box-shadow: -10px 0px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(10px);

}

.sidebar li {
  width: 100%;
}

.sidebar a {
  width: 100%;
}

nav {
  color: #fff;
  padding: 10px 10px 10px 0px;
  display: flex;
  justify-content: space-between;
}

nav ul {
  width: 100%;
  list-style: none;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

nav li {
  height: 50px;

}

nav a {
  height: 100%;
  padding: 0px 30px 0px 0px;
  text-decoration: none;
  display: flex;
  align-items: center;
  color: #fff;

}

nav a:hover {
  /* color: #e54d07; */
  text-decoration: underline;
}

nav li:first-child {
  margin-right: auto;
}

.menu-button {
  display: none;
}

@media(max-width: 960px) {
  .hideOnMobile {
    display: none;
  }

  .menu-button {
    display: block;

  }
}


.nav-end {
  text-align: center;
}

.nav-end-text {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 500;
  font-size: 16px;
  line-height: 27.2px;
  color: #FFFFFF;
  opacity: 80%;
  display: flex;
  justify-content: center;
  align-items: center;

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
