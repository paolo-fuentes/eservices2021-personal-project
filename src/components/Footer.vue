<template>
  <div class="footer">
      <div class="footer-content">
        <h3>The Beacon Steakhouse</h3>
      
          <ul class="socials">
            <li><a href="#"><i class="fa fa-facebook"></i></a></li>
            <li><a href="#"><i class="fa fa-twitter"></i></a></li>
            <li><a href="#"><i class="fa fa-google-plus"></i></a></li>
            <li><a href="#"><i class="fa fa-youtube"></i></a></li>
            <li><a href="#"><i class="fa fa-linkedin-square"></i></a></li>
          </ul>
      </div>
      <div class="footer-bottom">
        <p>copyright &copy;2021 eServices. designed by <span>Paolo Fuentes</span></p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

.footer {
  background: #320911;
  height: 20vh;
  width: auto;
  padding-top: 20px;
  color: #fff
}

.footer-content {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
}

.footer-content h3 {
  font-size: 1.8rem;
  font-weight: 400;
  text-transform: capitalize;
  line-height: 3rem;
}

.footer-content {
  max-width: 500px;
  margin: 10px auto;
  line-height: 28px;
  font-size: 14px;
}

.socials {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
}

.socials li {
  margin: 0 10px;
}

.socials a {
  text-decoration: none;
  color: #fff;
}

.socials a i {
  font-size: 1.1rem;
  transition: color .4s ease;
}

.socials a:hover i {
  color: #ecd7ad;
}

.footer-bottom {
  background: #320911;
  width: 100vw;
  padding: 20px 0;
  text-align: center;
}

.font-bottom p {
  font-size: 14px;
  word-spacing: 2px;
  text-transform: capitalize;
}

.footer-bottom span {
  opacity: .4;
  font-weight: 200;
}

</style>

<!-- https://www.youtube.com/watch?v=zdA3qZNH1vc&ab_channel=CodeOpacity -->

