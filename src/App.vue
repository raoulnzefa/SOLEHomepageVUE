<template>
  <div class="App">
    <header class="App-header">
      <picture>
        <source srcset="./assets/SOLEMapHeaderSlim.png" media="(min-width: 800px)">
        <img src="./assets/SOLEMapHeaderFull.png" alt="SOLE Map Header" />
      </picture>
    </header>
      <main class="App-main">
        <h1>Welcome to SOLE</h1>
          <p>SOLE provides an easy-to-use online shopping and community experience to rediscover and connect with local shops, services and amenities.</p>
          <p>Download the app today to browse and shop, book activities or events, find a local service, join a group, keep up with local news or go on a trail.</p>
  
            <div class="App-download-container">
              <a href="https://apps.apple.com/us/app/sole-scot/id1553277615" target="_blank">
              <img alt="Apple Store download button" src="./assets/AppleStore.png"/>
              </a>

              <a href="https://play.google.com/store/apps/details?id=com.ocs.sole.app" target="_blank">              
              <img alt="Google Play Store download button" src="./assets/GoogleStore2.png"  />
              </a>
            </div>

          <p>The SOLE app is packed with special offers, competitions and promotions.</p>
          <p>Local businesses now have the chance to trade together online to their community as well as in their physical spaces. </p>
          <p>To start using SOLE as an individual or a business, either click on your area link below or register on the app today.</p>
         
          <h3>SOLE is available for the following East Lothian regions:</h3>
            <div class="App-county-container">
                <div class="App-county-item">
                  <a href="https://www.sole.scot/Dunbar">
                    <!-- {/* link to Dunbar town home page */} -->
                    <img alt="Dunbar map icon" class="App-county-logo" src="./assets/DunbarMapIcon.png" />
                    <p>Dunbar and East Linton</p> 
                  </a>
                </div>
                <div class="App-county-item">
                  <a href="https://www.sole.scot/Haddington">
                    <!-- {/* link to Haddington town home page */} -->
                    <img alt="Haddington map icon" class="App-county-logo" src="./assets/HaddingMapIcon.png"  />
                    <p>Haddington and Lammermuir</p> 
                  </a>
                </div>
                <div class="App-county-item">
                  <a href="https://www.sole.scot/Musselburgh">
                    <!-- {/* link to Musselburgh town home page */} -->
                    <img alt="Musselburgh map icon" class="App-county-logo" src="./assets/MusselMapIcon.png"  />
                    <p>Musselburgh</p> 
                  </a>
                </div>
                <div class="App-county-item">
                  <a href="https://www.sole.scot/NorthBerwick">
                    <!-- {/* link to North Berwick town home page */} -->
                    <img alt="North Berwick map icon" class="App-county-logo" src="./assets/NBMapIcon.png"  />
                    <p>North Berwick Coastal</p> 
                  </a>
                </div>
                <div class="App-county-item">
                  <a href="https://www.sole.scot/PrestonSetonGosford">
                    <!-- {/* link to Preston Seton Gosford town home page */} -->
                    <img alt="Prestonpans map icon" class="App-county-logo" src="./assets/PrestonMapIcon.png"  />
                    <p>Preston, Seton and Gosford</p> 
                  </a>
                </div>
                <div class="App-county-item">
                  <a href="https://www.sole.scot/Tranent">
                    <!-- {/* link to Tranent town home page */} -->
                    <img alt="Tranent map icon" class="App-county-logo" src="./assets/FaSideMapIcon.png"  />
                    <p>Fa'side</p> 
                  </a>
                </div> 
            </div>
            <hr />
            <footer class="App-footer">
              <div class="App-footer-container">
              <div class="App-footer-item-gov">
                    <img alt="UK Government Logo" class="App-footer-logo-UKGov" src="./assets/UKGovLogo2.png"  />
                    <p class="App-footer-logo-text">This project is funded by the UK Government through the UK Community Renewal Fund.</p> 
                </div>
                <div class="App-footer-item-elc">
                    <img alt="East Lothian Council Logo" class="App-footer-logo-ELC" src="./assets/ELCLogo.png"  />
                </div> 
              </div>
            </footer>
      </main>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;700&display=swap');

* {
  text-align: center;
  line-height: 1.2;
  font-family: 'Source Sans Pro', sans-serif;
  box-sizing: border-box;
  /* This font-family has been imported from Google fonts. */
}

body {
  margin: 0;
}

.App { 
  background-color: white;
  min-height: 100vh;
  color: #6e4d76;
  /* color code taken from SOLE marketing docs */
}

.App-header img {
  width: 100vw; 
}

.App-main {
  padding: 0 20px;
}

h1 {
  margin: 0;
}

.App-download-container {

}

.App-download-container img {
  height: 50px;
  margin: 20px 10px 10px 10px;
}

.App-download-container img:hover {
  cursor: pointer;
}

.App-county-container {
  display: grid;
  grid-template-columns: repeat(6, auto);
  grid-gap: 15px;
  justify-content: center;
  width: 90vw;
  margin: 20px auto 50px auto;
}

.App-county-item {
  max-width: 140px; 
}

.App-county-item p {
  margin: 0;
  font-size: 16px;
  color: #6E4D76;
  /* color code taken from SOLE marketing docs */
  line-height: normal;
}

.App-county-item a {
  margin: 0;
  text-decoration: none;
}

.App-county-logo {
  height: 100px;
}

.App-footer-container {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  grid-gap: 15px;
  width: 40vw;
  margin: 40px auto 50px auto;
}

.App-footer-item-gov {
  text-align: start;
  align-self: center;
}

.App-footer-item-elc {
  text-align: end;
  align-self: center;
}

.App-footer-logo-UKGov {
  height:50px;
}

.App-footer-logo-ELC {
  height:65px;
}

.App-footer-logo-text {
  margin: 0;
  text-align: start;
  font-size: 12px;
  color: black;
}

hr {
  border-top: 1px solid #6E4D76;
  width: 90vw;
}

/* RESPONSIVE RULES FOR VIEWING ON MOBILE DEVICES */

@media (max-width: 1200px) {
  .App-footer-container {
    grid-gap: 10px;
    width: 50vw;
  }
}
  

@media (max-width: 840px) {
  .App-county-container {
    grid-template-columns: repeat(3, auto);
    grid-gap: 20px;
  }
  .App-footer-container {
    grid-gap: 10px;
    width: 70vw;
  }
  .App-footer-logo-ELC {
    height:60px;
  }
}

@media (max-width: 450px) {
  .App-main {
    padding: 0 15px;
}

  .App-county-container {
    grid-template-columns: repeat(2, auto);
    grid-gap: 10px;
  }

  .App-download-container img {
    display: block;
    width: 150px;
    height: auto;
    margin: 10px auto;
  }
  .App-footer-container {
  width: 85vw;
  margin: 40px auto 50px auto;
  }
  .App-footer-logo-ELC {
  height:50px;
  }
}
</style>