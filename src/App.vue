<script setup>
import Footer from './components/Footer.vue';
import HotelPolicy from './components/HotelPolicy.vue';
import Navbar from './components/Navbar.vue';
import Overview from './components/Overview.vue';
import ShowRoom from './components/ShowRoom.vue';
import SimilarStays from './components/SimilarStays.vue';
</script>

<template>
  <header>



    <div>
      <Navbar />
    </div>


  </header>

  <main>
    <div>
      <Overview />
    </div>
    <div>
      <ShowRoom />
    </div>
    <div>
      <HotelPolicy/>
    </div>
    <div>
      <SimilarStays />
    </div>
    <div>

    </div>
  </main>
  <footer>
    <Footer />
  </footer>
</template>

<style scoped>
/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>
