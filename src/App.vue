<script setup>
import Footer from './components/Footer.vue';
import HotelPolicy from './components/HotelPolicy.vue';
import Navbar from './components/Navbar.vue';
import Ratings from './components/Ratings.vue';
import Room from './components/Room.vue';
import SimilarStays from './components/SimilarStays.vue';
import Facilities from './components/Facilities.vue';
import Overview from './components/Overview.vue';
</script>

<template>
  <header>
    <div>
      <Navbar />
    </div>


  </header>

  <main>
    <div>
      <Overview/>
    </div>
    <div>
      <Room />
    </div>
    <div>
      <Ratings />
    </div>
    <div>
      <Facilities/>
    </div>
    <div>
      <HotelPolicy />
    </div>
    <div>
      <SimilarStays />
    </div>
    <div>
      <Footer />
    </div>
  </main>
</template>

<style scoped></style>
