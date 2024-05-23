<script setup>
    import { RouterLink } from 'vue-router';
</script>

 
<template>
    <footer>
        <div class="card">
            <div class="column">
                <h1>Sofie S. Fischer</h1>
                <p class="p1">Web designer, grafisk designer, UX-designer baseret i Esbjerg, Danmark.</p>
            </div>
            <div class="column">
                <div class="column">
                    <nav>
                        <ul class="nav-routes">
                            <ul class="nav-routes">
                                <li class="nav-links"><a href="#scrollTilHjem">Tilbage til start</a></li>
                                <li class="nav-links"><a href="#scrollTilOm">Om mig</a></li>
                                <li class="nav-links"><a href="#scrollTilProjekter">Mine projekter</a></li>
                                <li class="nav-links"><a href="#scrollTilKontakt">Kontakt</a></li>
                            </ul>
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

    .p1{
        padding-bottom: 3vh;
        font-family: 'Raleway', sans-serif;
        font-size: 16px;
        margin-left: 25px;
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
