<template>
  <Navbar />
  <div class="landing">

    <div class="landText">
      <h3 class='mainHeader'>Welcome to The Beacon</h3>
      <p class='mainSubheader'>Serving Fire-Grilled Steaks since 1970</p>
    </div>

  </div>

  <div class='about'>
    <h4 class='aboutText'>DINING WITH STYLE IN</h4>
    <h3 class='aboutText'>THE BEST STEAKHOUSE IN TOWN</h3>
    <p class='mainSubheader'>Just like a well-cooked steak, the restaurant boasts of masculine and old-world charm. It incorporates the same design elements of original locations in New York, such as a long, mahogany solid wood bar, wooden planked floors, wood wainscoting, alabaster chandeliers and mosaic tile ceiling reminiscent of the original Gustavino tile ceiling of the first location in New York.</p>
    <router-link to="/about"><button class='button homeButton'>LEARN MORE</button></router-link>
  </div>

  <div class="featured">
    <h3 class='featuredText'>As Featured On</h3>
    <div class="logos">
      <img class='logoImage' src='../assets/abc.png' />
      <img class='logoImage' src='../assets/cnn.jpg' />
      <img class='logoImage' src='../assets/netflix.png'/>
      <img class='logoImage' src='../assets/tripadvisor.jpg'/>
    </div>

  </div>
  <Footer />

</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  margin: 0;
  padding: 0;
  color: #D3D3D3;
}

.landing {
  background: linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url("../assets/steakhome.jpg");

  /* Full height */
  height: 90vh;

  /* Center and scale the image nicely */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.landText {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.mainHeader {
  font-size: 60px;
  margin-bottom: 10px;
}

.mainSubheader {
  font-size: 30px;
  margin-bottom: 20px;
}

.button {
  border: none;
  color: white;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}

.homeButton {
  background-color: transparent; 
  color: #D3D3D3; 
  border: 2px solid #ecd7ad;
  font-size: 16px;
  font-weight: 600;
  margin-top: 30px;

}

.homeButton:hover {
  background-color: #ecd7ad;
  border: 2px solid #ecd7ad;
  color: #4f0c19;
}

.about {
  padding: 40px 0px 60px 0px;
  height: 100%;
  background-color: #4f0c19;

  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.about .mainSubheader {
  font-size: 16px;
  margin: 0 200px;
  line-height: 2;
}

.aboutText {
  display: flex;
  justify-content: center;
  color: white;
  font-size: 30px;
  padding-bottom: 20px;
}

.featured {
  padding: 40px 0px 70px 0px;
  height: 100%;
  background-color: #ecd7ad; 
  
}

.logos {
  display: flex;
  justify-content: center;
  align-items: center;
}

.featuredText {
  display: flex;
  justify-content: center;
  color: black;
  font-size: 40px;
  padding-bottom: 20px;
}

.logoImage {
  width: 16%;
  height: auto;
}

</style>
