<template>
<div class="App">
      <header class="App-header">
        <img alt="SOLE map header" src="./assets/SOLEMapHeader2.png" />
      </header>
      <main class="App-main">
        <h1>Welcome to SOLE</h1>
          <p>SOLE is an app for the East Lothian community.</p>
          <p>SOLE provides an easy-to-use online shopping and community experience to rediscover and connect with local shops, services and amenities.</p>
          <p>Download the app today to browse and shop, book activities or events, find a local service, join a group, keep up with local news or go on a trail.</p>
          <p>The SOLE app is packed with special offers, competitions and promotions.</p>

            <div class="App-download-container">
              <img alt="Apple Store download button" src="./assets/AppleStore.png"  />
              <!-- {/* link to Apple App Store URL */} -->
              <img alt="Google Play Store download button" src="./assets/GoogleStore.png"  />
              <!-- {/* link to Google Play Store URL */} -->
            </div>

          <p>Local businesses now have the chance to trade together online to their community as well as in their physical spaces. </p>
          <p>If you are a business you can register here:</p>
          <button>Register Now</button>
          <!-- {/* link to business registration page */} -->
          <h3>SOLE is available for the following East Lothian regions:</h3>
          <div class="App-county-container">
              <div class="App-county-item">
                <a href="">
                  <!-- {/* link to Dunbar town home page */} -->
                  <img alt="Dunbar map icon" class="App-county-logo" src="./assets/DunbarMapIcon.png" />
                  <p>Dunbar and East Linton</p> 
                </a>
              </div>
              <div class="App-county-item">
                <a href="">
                   <!-- {/* link to Haddington town home page */} -->
                  <img alt="Haddington map icon" class="App-county-logo" src="./assets/HaddingMapIcon.png"  />
                  <p>Haddington and Lammermuir</p> 
                </a>
              </div>
              <div class="App-county-item">
                <a href="">
                   <!-- {/* link to Musselburgh town home page */} -->
                  <img alt="Musselburgh map icon" class="App-county-logo" src="./assets/MusselMapIcon.png"  />
                  <p>Musselburgh</p> 
                </a>
              </div>
              <div class="App-county-item">
                <a href="">
                   <!-- {/* link to North Berwick town home page */} -->
                  <img alt="North Berwick map icon" class="App-county-logo" src="./assets/NBMapIcon.png"  />
                  <p>North Berwick Coastal</p> 
                </a>
              </div>
              <div class="App-county-item">
                <a href="">
                   <!-- {/* link to Preston Seton Gosford town home page */} -->
                  <img alt="Prestonpans map icon" class="App-county-logo" src="./assets/PrestonMapIcon.png"  />
                  <p>Preston, Seton and Gosford</p> 
                </a>
              </div>
              <div class="App-county-item">
                <a href="">
                   <!-- {/* link to Tranent town home page */} -->
                  <img alt="Tranent map icon" class="App-county-logo" src="./assets/FaSideMapIcon.png"  />
                  <p>Fa'side</p> 
                </a>
              </div> 
          </div>
      </main>
      <!-- {/* Application FOOTER component HTML code will need to be added here. */} -->
    </div>
  
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" /> -->
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;700&display=swap');

* {
  text-align: center;
  line-height: 2;
  font-family: 'Source Sans Pro', sans-serif;
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

.App-download-container {
  margin: 15px 0px; 
}

.App-download-container img {
  height: 50px;
  margin: 10px;
}

.App-download-container img:hover {
  cursor: pointer;
}

.App button {
  padding: 5px 20px;
  background-color: #6E4D76;
  color: white;
  border: solid 1px white;
  border-radius: 5px;
  cursor: pointer;
  margin: 15px 0px;
}

.App button:hover {
  background-color: #493557;
  /* color code taken from SOLE marketing docs */
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
  line-height: normal;
}

.App-county-item a {
  margin: 0;
  text-decoration: none;
}

.App-county-logo {
  height: 125px;
}

/* RESPONSIVE RULES FOR VIEWING ON MOBILE DEVICES */

@media (max-width: 840px) {
  .App-county-container {
    display: grid;
    grid-template-columns: repeat(3, auto);
    grid-gap: 20px;
  }
}

@media (max-width: 450px) {
  .App-main {
  padding: 0 15px;
}

  .App-county-container {
    display: grid;
    grid-template-columns: repeat(2, auto);
    grid-gap: 20px;
  }

  .App-download-container img {
    display: block;
    width: 150px;
    height: auto;
    margin: 10px auto;
  }
}
</style>