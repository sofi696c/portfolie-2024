<template>
  <header :class="{ 'sticky': isSticky }">
    <nav class="container">
      <div class="porfolie">
        <h1 class="logo">Sofie S. Fischer</h1>
      </div>

      <ul class="nav-routes">
        <li class="nav-links"><a href="#scrollTilHjem">Hjem</a></li>
        <li class="nav-links"><a href="#scrollTilOm">Om mig</a></li>
        <li class="nav-links"><a href="#scrollTilProjekter">Mine projekter</a></li>
        <li class="nav-links"><a href="#scrollTilKontakt">Kontakt</a></li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const isSticky = ref(false);

// Function to handle scroll event
const handleScroll = () => {
  isSticky.value = window.scrollY > 0;
};

// Listen for scroll event
window.addEventListener('scroll', handleScroll);
</script>

<style scoped>
header {
  background-color: white;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  height: 8vh;
  transition: 0.3s; /* Add smooth transition for sticky effect */
}

.sticky {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
}

nav {
  display: flex;
  align-items: center;
  padding: 25px 16px;
}

.logo {
  font-size: 30px;
  font-weight: 700;
  color: #965151;
  font-family: pacifico;
  
}


.nav-routes {
  display: flex;
  flex: 1;
  justify-content: flex-end;
  gap: 12px;
  list-style: none;
}

.nav-routes a {
  text-decoration: none;
  color: inherit;
}

.nav-routes a:hover {
  color: #965151;
  cursor: pointer;
  text-decoration: underline;
  transition: 0.4s;
}

@media screen and (max-width: 768px) {
  .nav-routes {
    display: none;
  }

  nav {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 25px 16px;
  }
}
</style>
