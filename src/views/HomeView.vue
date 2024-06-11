<template>
  <div class="hjem-site">
    <div id="scrollTilHjem" class="velkommen">
      <div class="velkommen-card" :class="{ expanded: isExpanded }">
        <div class="column">
          <div class="mig-billede">
            <div class="billede">
              <img class="mig-img" src="../assets/portfo-billede.png" alt="billede af mig">
            </div>
          </div>
        </div>
        <div class="column">
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

    <div id="scrollTilOm" class="om-mig">
      <h1>Om mig</h1>
      <div class="cv-card">
        <div class="cv-column">
          <h3>Se denne korte video, <br>
            hvor jeg fortæller lidt <br>
            om mig selv!
          </h3>
          <button class="cv-button" onclick="window.open('./cv-FINAL.pdf','_blank')">Download mit CV her!</button>
        </div>
        <div class="column">
          <div class="card-content">
          </div>
          <div class="video-container">
            <iframe width="100%" height="300vh" src="https://www.youtube.com/embed/Sk-EPj8-Lvw" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>

    <div id="scrollTilProjekter" class="projekter">
      <h1>Mine projekter</h1>
      <div class="card-container">
        <div class="projekt-card" v-for="card in Cards" :key="card.id">
          <Card 
            :title="card.title" 
            :description="card.description"
            :image="card.image"
          />
        </div>
      </div>  
    </div>

    <div id="scrollTilKontakt" class="kontakt">
      <div class="kontakt-card">
        <div class="column">
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
import Card from '../components/Card.vue';
import imageOne from '../assets/t1.png';
import imageTwo from '../assets/trapholt-folder-forside.png';
import imageThree from '../assets/Kleen-Keester.png';
import imageFour from '../assets/reops.png';
import imageFive from '../assets/coffee-website.png';
import imageSix from '../assets/invi1.png';

export default {
  name: 'App',
  components: {
    Card
  },
  data() {
    return {
      Cards: [
        { 
          id: 1, 
          title: 'Trapholt kunst & design museum (website)', 
          description: 'Mit første semesters eksamensprojekt fokuserede på at redesigne hjemmesiden for Trapholt med fokus på responsivt design. Gennem en dybdegående undersøgelse af museets behov og brugernes forventninger udviklede jeg, i samarbejde med min gruppe, en ny hjemmeside.',
          image: imageOne   
        },
        { 
          id: 2, 
          title: 'Trapholt kunst & design museum (graphics)', 
          description: 'I mit første semesters eksamensprojekt skabte jeg en serie infografikker til Trapholt Kunst og Design Museum. Disse visuelle repræsentationer af museets udstillinger og kunsterne bag, gjorde kompleks information letforståelig og engagerende. Resultatet var en serie infografikker, der formidlede museets unikke identitet og tiltrak besøgende på en visuelt tiltalende måde.',
          image: imageTwo
        },
        { 
          id: 3, 
          title: 'Kleen Keester', 
          description: 'I forhold til Kleen Keester blev der udviklet en maskot til virksomheden samt en hjemmeside-mock-up i Adobe XD. Gennem kreativ brainstorming og designprocesen blev en indbydende og mindeværdig maskot skabt, der repræsenterede virksomhedens værdier og brandidentitet på en charmerende måde. Den tilhørende hjemmeside-mock-up blev designet med fokus på brugervenlighed, æstetik og funktionalitet med det formål at tiltrække og engagere besøgende på en intuitiv måde.',
          image: imageThree
        },
        {
          id: 4,
          title: 'ReOps',
          description: 'ReOps er en online jobportal, hvor brugeroplevelsen har højeste prioritet. Gennem en omhyggelig designproces blev der udviklet en prototype af appen med funktioner, der virker. Med fokus på brugervenlighed og intuitivt design blev hver funktion skabt med det formål at optimere jobansøgningsprocessen for både jobsøgere og virksomheder. ReOps tilbyder en sømløs og effektiv platform, der gør det nemt for brugere at navigere og finde relevante jobmuligheder.',
          image: imageFour
        },
        {
          id: 5,
          title: 'Mocha More',
          description: 'Mocha More er en website designet til en hyggelig café. Fokusset var på at skabe en tiltalende hjemmeside med en balance mellem design og udvikling. Ved at kombinere æstetik og funktionalitet blev hjemmesiden skabt med det formål at tiltrække og engagere besøgende. Fra brugervenlig navigation til visuelt tiltalende designelementer blev hver detalje omhyggeligt udformet for at skabe en behagelig onlineoplevelse for caféens kunder.',
          image: imageFive
        },
        {
          id: 6,
          title: 'Invitaion',
          description: 'Denne invitation er skabt med omhu og opmærksomhed på detaljerne, i tæt samarbejde med fødselaren selv. Vores fokus har været på at afspejle fødselarens personlighed og stil gennem valg af design, farver og layout. Vi har arbejdet hårdt på at sikre, at invitationen udstråler elegance og festlighed, samtidig med at den er informativ og letlæselig. Fra valg af skrifttype til billedmateriale har vi stræbt efter at skabe en invitation, der skaber forventning og glæde hos gæsterne. Vi håber, at du vil nyde resultatet og glæde dig til at deltage i fejringen af denne særlige dag.',
          image: imageSix
        }
      ]
    }
  }
}
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

  }
  
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
    height: 65vh;
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
  

  h1 {
    font-family: 'raleway', sans-serif;
    font-size: 35px;
    margin-bottom: 5%;
  }

  h2 {
    font-family: 'raleway', sans-serif;
    font-size: 35px;
    margin-bottom: 5%;
  }

 

  .p1 {
    font-family: 'Raleway', sans-serif;
    text-align: left;
    padding-bottom: 2.5%;
    width: 90%;
    line-height: 1.6; /* Adjust line-height for increased spacing */
  }



  .projekter {
  display: flex;
  flex-direction: column;
  align-items: center !important;
  justify-content: center;
  width: 100%;
  margin: 0 auto;
  padding: 10% 16px;
}

.card-container {
  display: flex;
  flex-direction: column;
  align-items: center; /* Center items horizontally */
  justify-content: center; /* Center items vertically */
}

.projekt-card {
  display: flex;
  justify-content: center; /* Center content horizontally */
  width: 100%;
}




  

  h3 {
    font-family: 'raleway', sans-serif;
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
    font-family: 'raleway', sans-serif;
    text-align: left;
    padding-bottom: 20px;
    width: fit-content;
    line-height: 2.5; /* Adjust line-height for increased spacing */
  }

  .p3 {
    font-family: 'raleway', sans-serif;
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

  .card-container {
    flex-direction: column;
    align-items: center; /* Center items horizontally */
  }

  .projekt-card {
    justify-content: center; /* Center content horizontally */
  }
}



  .mine-projekter {
    padding: 10% 16px; /* Adjust padding as needed */
    flex-direction: column;
  }


  .projekt-card {
    flex-direction: column; /* Change flex-direction to column */
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
    height: auto !important;
    width: 80%;
    justify-content: center;
    align-items: center;
    background-color: rgba(255, 255, 255, 0.60); /* White background color with 0.75 opacity */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }





</style>




  