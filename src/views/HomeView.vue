<template>
  <div class="hjem-site">
<!--     <div class="background-overlay"></div> 
    <div class="swirl-img"></div>
 -->
    <div class="velkommen">
      <div class="velkommen-card" :class="{ expanded: isExpanded }">
          <!-- Content for the first column -->
        <div class="column">  
          <div class="mig-billede">
            <div class="billede">
              <img class="mig-img" src="../assets/portfo-billede.png" alt="billede af mig">
            </div>
          </div> 
        </div>      

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <h1>Velkommen til mit univers!</h1>
            <p class="p1"> Jeg er Sofie, en passioneret multimediedesign-studerende 
              med en passion for at skabe engagerende og intuitive brugeroplevelser. 
              Min kreative rejse inden for UX og front-end-development er fyldt med farverige 
              ideer og spændende udfordringer. Gennem min portefølje inviterer jeg dig til at 
              udforske en verden af ​​kreativitet, hvor æstetik og funktionalitet forenes til at 
              skabe magi på skærmen.
            </p>

            <p class="p1">Lad mig tage dig med på en rejse gennem min vision og ekspertise inden
               for UX og front-end-development.
            </p>

        </div>
      </div>
    </div>

    <div class="om-mig">

    <h1>Om mig</h1>
      <div class="cv-card">
        <div class="cv-column">
          <!-- Content for the first column -->
          <h3>
            Se denne korte video, <br>
            hvor jeg fortæller lidt <br>
            om mig selv!
          </h3>

          <button class="cv-button" onclick="window.open('./cv-FINAL.pdf','_blank')">Download mit CV her!</button>

        </div>

        <div class="column">
          <div class="card-content">
            <!-- Other content within the card -->
          </div>  

          <!-- YouTube embed code -->
          <div class="video-container">
            <iframe width="100%" height="300vh" src="https://www.youtube.com/embed/Sk-EPj8-Lvw" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>

      </div>

    </div>


    <div id="mine-projekter" class="projekter">
      <h1>Mine projekter</h1>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>Trapholt kunst & design museum (website)</h2>
          <p class="p1"> Mit første semesters eksamensprojekt fokuserede på at redesigne hjemmesiden
            for Trapholt med fokus på responsivt design. Gennem en dybdegående 
            undersøgelse af museets behov og brugernes forventninger udviklede jeg, i samarbejde med min gruppe,
            en ny hjemmeside. </p>
            <!-- Projektetintegrerede en intuitiv navigation, æstetisk appel og nøjagtig præsentation af museets 
            kunstsamlinger og arrangementer. At skabe en brugercentreret oplevelse var kernen i projektet, 
            hvilket resulterede i en hjemmeside, der ikke kun fremviste museets unikke identitet, 
            men også tiltrak og engagerede besøgende på tværs af digitale platforme. -->

<!--         <router-link to="/trapholtweb">Se mere -->
          <button class="expand-button">Se mere</button>
<!--         </router-link> -->
          

        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/t1.png" alt="Billede af Trapholts hjemmeside" class="t-img">
                <img src="../assets/t3.png" alt="Billede ad Trapholts hjemmeside" class="t-img">
              </div>
            </div>  
        </div>
      </div>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>Trapholt kunst & design museum (graphics)</h2>
          <p class="p1">I mit første semesters eksamensprojekt skabte jeg en serie infografikker 
            til Trapholt Kunst og Design Museum. Disse visuelle repræsentationer af museets udstillinger og
            kunsterne bag, gjorde kompleks information letforståelig og engagerende. 
            Resultatet var en serie infografikker, der formidlede museets unikke identitet og tiltrak 
            besøgende på en visuelt tiltalende måde.</p>


             
          <button class="expand-button">Se mere</button>
        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/trapholt-folder-forside.png" alt="Billede af Trapholts folder" class="trifold-img">
                <img src="../assets/ditzel2.png" alt="Billede af ditzel" class="ditzel-img">
              </div>
            </div>  
        </div>
      </div>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>Kleen Keester</h2>
          <p class="p1"> I forhold til Kleen Keester blev der udviklet en maskot til virksomheden
            samt en hjemmeside-mock-up i Adobe XD. Gennem kreativ brainstorming og designprocesen
            blev en indbydende og mindeværdig maskot skabt, der repræsenterede virksomhedens værdier
            og brandidentitet på en charmerende måde.</p>

          <p class="p1">Den tilhørende hjemmeside-mock-up blev
            designet med fokus på brugervenlighed, æstetik og funktionalitet med det formål at
            tiltrække og engagere besøgende på en intuitiv måde.</p>
             
          <button class="expand-button">
            Se mere
          </button>
        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/Kleen-Keester.png" alt="Billede af kleen keesters hjemmeside" class="kleen-keester-img">
              </div>
            </div>  
        </div>
      </div>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>ReOps</h2>
          <p class="p1">ReOps er en online jobportal, hvor brugeroplevelsen har højeste prioritet. 
            Gennem en omhyggelig designproces blev der udviklet en prototype af appen med funktioner, 
            der virker. Med fokus på brugervenlighed og intuitivt design blev hver funktion skabt 
            med det formål at optimere jobansøgningsprocessen for både jobsøgere og virksomheder. 
            ReOps tilbyder en sømløs og effektiv platform, der gør det nemt for brugere at navigere 
            og finde relevante jobmuligheder.</p>

             
          <button class="expand-button">Se mere</button>
        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/reops.png" alt="Billede af ReOps" class="reops-img">
                <img src="../assets/reops-miro.jpeg" alt="Billede af miro" class="reops-img">
              </div>
            </div>  
        </div>
      </div>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>Mocha More </h2>
          <p class="p1">Mocha More er en website designet til en hyggelig café. Fokusset var på at
             skabe en tiltalende hjemmeside med en balance mellem design og udvikling. Ved at
              kombinere æstetik og funktionalitet blev hjemmesiden skabt med det formål at tiltrække
               og engagere besøgende. Fra brugervenlig navigation til visuelt tiltalende designelementer
                blev hver detalje omhyggeligt udformet for at skabe en behagelig onlineoplevelse for
                 caféens kunder.</p>

             
          <button class="expand-button">Se mere</button>
        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/coffee-website.png" alt="Billede af coffee website" class="coffee-img">
                <img src="../assets/coffee.png" alt="Billede af coffe website" class="coffee-img">
              </div>
            </div>  
        </div>
      </div>

      <div class="projekt-card">
        <div class="column">
          <!-- Content for the first column -->
          <h2>Invitaion</h2>
          <p class="p1">Denne invitation er skabt med omhu og opmærksomhed på detaljerne,
            i tæt samarbejde med fødselaren selv. Vores fokus har været på at afspejle fødselarens
            personlighed og stil gennem valg af design, farver og layout. Vi har arbejdet hårdt
            på at sikre, at invitationen udstråler elegance og festlighed, samtidig med at den
            er informativ og letlæselig. Fra valg af skrifttype til billedmateriale har vi
            stræbt efter at skabe en invitation, der skaber forventning og glæde hos gæsterne. 
            Vi håber, at du vil nyde resultatet og glæde dig til at deltage i fejringen af
            denne særlige dag.</p>
             
          <button class="expand-button">Se mere</button>
        </div>

        <div class="column">
          <!--Dette er højre side af cardet-->      
            <div class="projekt-billede">
              <div class="billede">
                <img src="../assets/invi1.png" alt="Billede af invitation" class="invi-img">
                <img src="../assets/invi2.png" alt="Billede ad invitation " class="invi-img">
              </div>
            </div>  
        </div>
      </div>

    </div>

  

    <div id="kontakt" class="kontakt">
        <div class="kontakt-card">
          <div class="column">
            <!-- Content for the first column -->
            <h2>Kontakt mig her!</h2>
            <p class="p1"> Tak fordi du besøger min portefølje! Hvis du har spørgsmål, 
                forslag eller vil diskutere et potentielt projekt, er jeg altid åben for at chatte. 
                Mit mål er at skabe meningsfulde og innovative løsninger, 
                og jeg tror på, at det bedste arbejde sker i samarbejde med andre.</p>

            <p class="p1">Du er velkommen til at kontakte mig, så vender jeg tilbage til dig så hurtigt som muligt. 
              Jeg sætter stor pris på din interesse og ser frem til at høre fra dig. 
              Lad os sammen omdanne idéer til virkelighed!</p>
          </div>

          <div class="column">
              <!-- Dette er højre side af cardet -->      
              <div class="info-card">
                  <div class="line"></div>
                  <div class="info">
                      <p class="p2"><i class="fas fa-phone"></i> <span class="icon-text">+45 42 26 52 03</span></p>
                      <p class="p2"><i class="fas fa-envelope"></i> <span class="icon-text">sofie.fischer@live.com</span></p>
                      <p class="p2"><i class="fab fa-linkedin"></i> <span class="icon-text">www.linkedin.com/in/sofie-fischer</span></p>
                  </div>
              </div>  
          </div>
        </div>
      </div>

  </div>
</template>

<script>


</script>


  
<style lang="scss">
.test{
  display: flex;
  justify-content: center;
  align-items: center;
  padding-top: 10px;
  
}

.fa-phone {
  color: #965151;
}

.fa-envelope {
  color: #965151;
}
.fa-linkedin {
  color: #965151;
}

.column {
    flex: 1;
    margin: 0 10px;
  }

  

.expand-button {
  background-color: #AA8484;
  border: none;
  color: white;
  font-size: 16px;
  padding: 10px 20px;
  z-index: 4;
  transition: background-color 0.3s, color 0.3s; /* Tilføjet transition for flydende overgangseffekt */
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
}

.expand-button:hover {
  background-color: #b69999; /* Ændrer baggrundsfarven ved hover */
  cursor: pointer;
  z-index: 4;
}

 


  .hjem-site {
    background-color: #F5F0F0; /* Set the background color */ 
    background-repeat: no-repeat; /* Prevent the background image from repeating */
    background-size: 90%; /* Cover the entire element with the background image */
    background-position: center; /* Center the background image */
    height: fit-content;
    /*     position: relative; 
     z-index: -1;  */
  
    .background-overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }

  .swirl-img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url('../assets/squiarl.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
    opacity: 0.5; /* Adjust the opacity as needed */
    z-index: -1;
  }

  .velkommen {
    display: flex;
    flex-direction: row; /* Change flex-direction to row */
    align-items: center; /* Vertically center items */
    justify-content: center;
    width: 100%; /* Adjust width as needed */
    margin: 0 auto;
    padding: 10% 16px;
    z-index: 2;
  }


  .velkommen-card {
    padding: 2% 0;
    display: flex;
    height: auto;
    width: 80%;
    justify-content: center;
    align-items: center;
    background-color: #d4dad4;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }

  .mig-billede {
  justify-content: center;
  width: auto; /* Increase the width to occupy more space */
  height: auto;
  display: flex;
  } 

  .billede {
    flex-wrap: wrap;
  }

  .mig-img {
    width: 80%;
    height: auto;
    width: 50vh;
    border: lightgray solid 1px;

  }

  .om-mig {
    display: flex;
    flex-direction: column; /* Change flex-direction to row */
    align-items: center; /* Vertically center items */
    justify-content: center;
    width: 100%; /* Adjust width as needed */
    margin: 0 auto;
    padding: 10vh 0;
  }

    .video-cv {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .cv-card {
    padding: 5vh;
    display: flex;
    height: auto;
    width: 80%;
    justify-content: center;
    align-items: center;
    background-color: rgba(255, 255, 255, 0.60); /* White background color with 0.75 opacity */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */

  }

  .cv-column {
    flex: 1;
    margin: 0 10px;
  }

  .cv-button {
    background-color: #AA8484; /* Green background color */
    border: none; /* Remove borders */
    color: white; /* White text color */
    font-size: 16px; /* Set the font size */
    cursor: pointer; /* Add a pointer cursor on mouse-over */
    padding: 10px 20px;
    transition: background-color 0.3s, color 0.3s; /* Tilføjet transition for flydende overgangseffekt */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }
  .cv-button:hover {
    background-color: #b69999; /* Ændrer baggrundsfarven ved hover */
    cursor: pointer;
    
  }
  .t-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;
  }

  .invi-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .trifold-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .ditzel-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .kleen-keester-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .reops-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .coffee-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  h1 {
    font-size: 35px;
    margin-bottom: 5%;
  }

  h2 {
    font-size: 35px;
    margin-bottom: 5%;
  }

 

  .p1 {
    text-align: left;
    padding-bottom: 2.5%;
    width: 90%;
    line-height: 1.6; /* Adjust line-height for increased spacing */
  }


  .mine-projekter {
    background-color: #F5F0F0; /* Set the background color */ 
    background-repeat: no-repeat; /* Prevent the background image from repeating */
    background-size: 90%; /* Cover the entire element with the background image */
    background-position: center; /* Center the background image */
    height: 2000px;
    position: relative; 
    z-index: -1;
  }


  .projekter {
    display: flex;
    flex-direction: column; /* Change flex-direction to row */
    align-items: center; /* Vertically center items */
    justify-content: center;
    width: 100%; /* Adjust width as needed */
    margin: 0 auto;
    padding: 10% 16px;
    z-index: 2;
  }
  

  .projekt-card {
    padding: 20px;
    display: flex;
    height: 5%;
    width: 70%;
    justify-content: center;
    align-items: center;
    background-color: #d4dad4; /* White background color with 0.75 opacity */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
    margin-bottom: 50px;
  }


  .projekt-billede {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
  }







  .projekt-card.expanded {
  height: 600px; /* Adjust the height as needed */
}






  h3 {
    font-size: 25px;
    margin-bottom: 15%;

  }
  .p1 {
    text-align: left;
    padding-bottom: 20px;
    width: 90%;
    line-height: 1.6; /* Adjust line-height for increased spacing */
  }

  .p2 {
    text-align: left;
    padding-bottom: 20px;
    width: fit-content;
    line-height: 2.5; /* Adjust line-height for increased spacing */
  }

  .p3 {
    text-align: left;
    padding-bottom: 20px;
    width: fit-content;
    line-height: 2.5; /* Adjust line-height for increased spacing */
  }

  .billede {
    display: flex;
    flex-direction: row; /* Change flex-direction to row */
    align-items: center; /* Vertically center items */
    justify-content: center;
    width: 100%; /* Adjust width as needed */
    margin: 0 auto;
    padding: 10% 16px;
    z-index: 2;
  }

  .billede-card {
    background-color: white;
    padding: 20px;
    display: flex;
    height: 500px;
    width: 80%;
    justify-content: center;
    align-items: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }

  .kontakt {
    display: flex;
    flex-direction: column; /* Change flex-direction to row */
    align-items: center; /* Vertically center items */
    justify-content: center;
    width: 100%; /* Adjust width as needed */
    margin: 0 auto;
    padding: 10% 16px;
  }

  .kontakt-card {
  padding: 20px;
  display: flex;
  height: 500px;
  width: 80%;
  justify-content: center;
  align-items: center;
  background-color: rgba(255, 255, 255, 0.60); /* White background color with 0.75 opacity */
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
}

.line {
  border: 1px solid #ccc;
  height: 350px;
  margin-top: 60px;
  width: 1px;
  margin-right: 30%;
}

.kontakt-info {
  display: flex;
  justify-content: flex-start;
  align-items: center;

}
.info-card {
  flex-direction: row;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

  .column {
    flex: 1;
    margin: 0 10px;
  }
}

.icon-text {
    margin-left: 8px; /* Adjust this value as needed for the desired space */
}

/* Media query for smaller screens */
@media (max-width: 768px) {


  
  .mig-img {
    display: none;

  }

  .column {
    flex-direction: column; /* Change flex-direction to column */
    height: auto; /* Allow the height to adjust based on content */
    justify-content: center;
  }
 


  .velkommen-card {
    flex-direction: column; /* Change flex-direction to column */
    height: auto; /* Adjust the height as needed */
    display: flex;

  }


  .om-mig {
    padding: 10% 16px; /* Adjust padding as needed */
  }

  .cv-card {
    flex-direction: column; /* Change flex-direction to column */
    height: 100%; /* Adjust the height as needed */
  }

  



  .mine-projekter {
    padding: 10% 16px; /* Adjust padding as needed */
    flex-direction: column;
  }


  .projekt-card {
    flex-direction: column; /* Change flex-direction to column */
    height: 700px; /* Allow the height to adjust based on content */
    overflow: auto;

  }

  .projekt-billede {
    justify-content: center; /* Center items horizontally */
    align-items: center; /* Center items vertically */
    height: auto;
    width: auto;
  }

  .kontakt {
    padding: 10% 16px; /* Adjust padding as needed */
  }

  .kontakt-card {
    flex-direction: column; /* Change flex-direction to column */
    height: auto !important; /* Allow the height to adjust based on content */
    overflow: auto;
  }

  .line{
    display: none;
  }

  .info-card {
    flex-direction: column; /* Change flex-direction to column */
    height: auto; /* Allow the height to adjust based on content */
  }
  
  .cv-column {
    justify-content: center;
  }

  .t-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

    
  }

  .invi-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .trifold-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .ditzel-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .kleen-keester-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;

  }

  .reops-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;


  }

  .coffee-img {
    width: 80%;
    height: auto;
    margin-bottom: 2.5%;


  }

  .cv-card {
    padding: 5vh;
    display: flex;
    height: auto;
    width: 80%;
    justify-content: center;
    align-items: center;
    background-color: rgba(255, 255, 255, 0.60); /* White background color with 0.75 opacity */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }


}


</style>




  