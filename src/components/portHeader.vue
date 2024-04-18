<script setup>
    import { RouterLink } from 'vue-router';
</script>

 
<template>
    <header>
        <nav class="container">
            <div class="porfolie">
                <h1>Sofie S. Fischer</h1>
            </div>

            <ul class="nav-routes ">
                <li><router-link to="/">Hjem</router-link></li>
                <li><router-link to="/om-mig">Om mig</router-link></li>
                <li><router-link to="/mine-projekter">Mine projekter</router-link></li>
                <li><router-link to="/kontakt">Kontakt</router-link></li>
            </ul>
        </nav>
    </header>
</template>




<style lang="scss" scoped>
    header {
        background-color: white;
    }

    nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;
    }

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  

</style>