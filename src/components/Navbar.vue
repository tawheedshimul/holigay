<template>
    <nav class="navbar">
        <div class="navbar-left">
            <div class="navbar-item">Holigay</div>
        </div>
        <div class="navbar-right">
            <div class="navbar-item">My Account</div>
            <div class="navbar-item">Guide</div>
            <button class="toggle-btn" @click="toggleSidebar">Toggle</button>
        </div>
    </nav>
</template>
  
<script setup>
import { ref } from 'vue';

const toggleMenu = ref(false);

function toggleSidebar() {
    toggleMenu.value = !toggleMenu.value;
}
</script>
  
<style scoped>
.navbar {
    background-color: #333;
    color: #fff;
    padding: 10px;
    display: flex;
    justify-content: space-between;
    opacity: 60%;
    display: fixed;
}

.navbar-right {
    display: flex;
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

@media (min-width: 1024px) {
    .navbar {
        padding: 10px 30px;
    }
}
</style>
  