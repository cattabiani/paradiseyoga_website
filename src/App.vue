<template>
  <div id="app">
    <div class="header-container">
      <h1>Paradise Yoga Center a Parma</h1>
    <div class="container">
      
      <!-- Left Column -->
      <div class="left-column">
        <!-- Main Logo -->
        <img src="./assets/logo.jpg" alt="Paradise Yoga Center Logo" class="main-logo" />

        <!-- Placeholder for Map -->
        <div class="map">
          <iframe
            width="100%"
            height="200"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3150.6825250058027!2d10.570523615383276!3d44.78854797910317!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x12d225fb301fc1eb%3A0xeefb747aa6730f52!2sVia%20Laudedeo%20Testi%204%2C%20Parma%20PR%2C%20Italy!5e0!3m2!1sen!2sus!4v1699051234567!5m2!1sen!2sus"
            frameborder="0"
            style="border:0;"
            allowfullscreen=""
            aria-hidden="false"
            tabindex="0"
          ></iframe>
        </div>
      </div>

      <!-- Right Column -->
      <div class="right-column">
        <!-- Sponsored Image and Text -->
        <div class="sponsor">
          <p>Con il patrocinio di:</p>
          <img src="./assets/AiCS.png" alt="Associazione Italiana Cultura e Sport Logo" class="sponsor-logo" />
        </div>

        <!-- Main Text Content -->
        <div class="main-text">
          <h3 class="date">da giovedì 7 novembre 2024</h3>

          <p class="calendar">
            <strong>CALENDARIO DELLE PRATICHE FINO AL 30 DICEMBRE 2024:</strong>
          </p>

          <div class="pratiche">
            <span class="yoga"><b>HATA YOGA</b></span><br />
            <span class="yoga"><b>(GIOVEDI’ alle 18,15)</b></span><br />
            <span class="yoga"><b>SWEET YOGA FLOW</b></span><br />
            <span class="yoga"><b>(SABATO alle 10,30)</b></span>
          </div>

          <p class="riequilibrio">
            RIEQUILIBRIO PSICO-FISICO SECONDO LA CULTURA E LA PRATICA YOGICA
          </p>

          <p class="prima-pratica">
            <strong>PRIMA PRATICA GRATUITA</strong>
          </p>

            <strong>Per tutte le informazioni:</strong><br />
            <address>
  Paradise Yoga Center<br />
  Via Laudedeo Testi 4, Parma PR, Italy<br />
  Phone: +39 334 657 5822<br />
  <a href="mailto:carlo.cattabiani@unipr.it">carlo.cattabiani@unipr.it</a>
</address>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
/* Overall layout */
#app {
  display: flex;
  justify-content: center;
  font-family: Arial, sans-serif;
  padding: 20px;
}

.header-container {
  display: flex;
  max-width: 1000px; /* Set a max-width for better layout */
  width: 100%;
  flex-direction: column;
}

.container {
  display: flex;
  max-width: 1000px; /* Set a max-width for better layout */
  width: 100%;
}

.left-column {
  flex: 1; /* Allow the left column to take up space */
  display: flex;
  flex-direction: column;
  align-items: center; /* Center items in the left column */
}

.right-column {
  flex: 2; /* Allow the right column to take up more space */
  padding-left: 20px; /* Space between columns */
}

.main-logo {
  width: 100%;
  max-width: 300px; /* Adjust logo size */
  margin-bottom: 20px; /* Space below the logo */
}

.map {
  width: 100%;
  height: 200px;
  background-color: #eee;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #666;
  margin: 20px 0; /* Space below the map placeholder */
  font-style: italic;
}

.sponsor {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 10px; /* Space below sponsor section */
}

.sponsor-logo {
  width: 150px;
  margin-top: 10px;
}

.main-text {
  text-align: left; /* Align text to the left */
}

.date {
  color: red; /* Change color to red */
}

.calendar {
  font-size: 1.2em;
  font-weight: bold;
  color: red; /* Make it red */
}

.pratiche {
  font-size: 1.5em; /* Make the practices larger */
  color: black; /* Set text color to black */
  margin: 10px 0; /* Margin for spacing */
  width: 100%; /* Take full width */
}

.yoga {
  color: black; /* Keep yoga text black */
}

.prima-pratica {
  font-size: 2em; /* Make this even bigger */
  font-weight: bold;
  color: red; /* Make it red */
  margin: 15px 0; /* Margin for spacing */
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .container {
    flex-direction: column; /* Stack on smaller screens */
    align-items: center; /* Center items */
  }

  .main-logo {
    margin-right: 0; /* Remove right margin on small screens */
  }

  .right-column {
    padding-left: 0; /* Remove left padding on small screens */
  }
}
</style>
