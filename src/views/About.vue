<template>
  <Navbar />
  <div class="aboutHeader">
      <h3 class='mainHeader'>ABOUT US</h3>
  </div>

  <div class=aboutText>
    <div class='content'>
      <h3 class='mainHeader'>What Makes Us Special?</h3>
    </div>

    <div class='paragraph'>
      <p class='mainSubheader'>Let your tastebuds get some love at I’m Angus, The Prime Steak House!</p>

      <p class='mainSubheader'>Treat yourself with the finest and Certified Angus Steak, fresh seafood, toothsome side dishes, and decadent desserts. All delicious food in one table at I’m Angus Steakhouse.</p>
      
      <p class='mainSubheader'>I’m Angus Steakhouse aims to raise the standard of excellence for a steakhouse to a whole new level. I’m Angus Steakhouse’s ultimate goal is to celebrate the ecstasy of extraordinary food platters and never-ending wine lists, in the company of friends and family.</p>
      
      <p class='mainSubheader'>I’m Angus Steakhouse is destined to offer a fine-dining experience featuring only the elite choice in prime beef with other tempting food varieties. We ensure to cater to a wide range of tasty salads, classy side dishes, and indulgent desserts. Can dining be fine without wine? We got that too! We have a hand-picked variety of the world’s best wines.</p>
      
      <p class='mainSubheader'>Being an affiliate of Chesa Bianca Swiss Restaurant, one of the city’s highly acclaimed and loved fine-dining restaurants, I’m Angus Steakhouse also presents a stylish and contemporary dining ambience. Luxury at every step! Every table of the house provides a truly comfortable and satisfying dining atmosphere.</p>
      
      <p class='mainSubheader'>What makes I’m Angus Steak House a foodie’s favourite?</p>
      
      <p class='mainSubheader'>The clear glass to the kitchen allows each guest to see the freshness of their food choices as the chef serves them straight off from the grill!</p>
    </div>
  </div>
  <Footer />
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'About',
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

.about {
  height: 80vh;
  background-color: #ecd7ad; 
}

.aboutHeader {
  background: linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url("../assets/about.jpg");

  /* Full height */
  height: 50vh;

  /* Center and scale the image nicely */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.content {
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
}

.aboutText {
  padding-top: 40px;
  height: 100%;
  background-color: #ecd7ad; 
}

.aboutText .mainHeader {
  font-size: 35px;
  margin-bottom: 10px;
  color: black;
  margin-bottom: 20px;
}

.aboutText .mainSubheader {
  font-size: 20px;
  color: #666666;
  padding-bottom: 30px;
}

.paragraph {
  margin: 0 15rem;
  padding-bottom: 30px;
}



</style>
