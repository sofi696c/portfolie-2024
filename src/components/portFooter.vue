<script setup>
    import { RouterLink } from 'vue-router';
</script>

 
<template>
    <footer>
        <div class="card">
            <div class="column">
                <h1>Sofie S. Fischer</h1>
                <p>Web designer, grafisk designer, UX-designer baseret i Esbjerg, Danmark.</p>
            </div>
            <div class="column">
                <div class="column">
                    <nav>
                        <ul class="nav-routes">
                            <li><RouterLink to="/hjem">Tilbage til toppen</RouterLink></li>
                            <li><RouterLink to="/om-mig">Om mig</RouterLink></li>
                            <li><RouterLink to="/mine-projekter">Mine Projekter</RouterLink></li>
                            <li><RouterLink to="/kontakt">Kontakt</RouterLink></li>
                        </ul>
                    </nav>
                </div>

                <div class="column">

                </div>

                <div class="column">

                </div>
                
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    footer {
        background-color: #AA8484;
        height: 30vh;
    }

    .card {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 100%;
    }
    
    .column {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
    }
    h1{
        padding-bottom: 3vh;
        font-family: 'Pacifico', cursive;
        font-size: 50px;
    }

    h4{
        padding-bottom: 1vh;
    }

    .logo {
        font-size: 24px;
        font-weight: 700;
        color: #965151;
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
        transition: 0.4s; /* Moved transition here for smoother effect */
    }

    .nav-routes a:hover {
        color: white;
        cursor: pointer;
        text-decoration: underline;
    }

    @media screen and (max-width: 768px) {
        .nav-routes {
            flex-direction: column;
            gap: 12px;
            list-style: none;
        }

        h1{
        padding-bottom: 3vh;
        font-family: 'Pacifico', cursive;
        font-size: 24px;
    }
      
    }
</style>
