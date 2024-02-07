<script setup>
import Footer from './components/Footer.vue';
import HotelPolicy from './components/HotelPolicy.vue';
import Navbar from './components/Navbar.vue';
import Overview from './components/Overview.vue';
import Ratings from './components/Ratings.vue';
import ShowRoom from './components/ShowRoom.vue';
import Room from './components/Room.vue';
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
      <Room />
    </div>
    <div>
      <Ratings />
    </div>
    <div>
      <HotelPolicy />
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

</style>
