<template>
  <div class="nav">
    <nav>
        <label class='logo'>The Beacon Steakhouse</label>
        <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/about">About</router-link></li>
        </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
    padding: 0;
    margin: 0;
    text-decoration: none;
    list-style: none;
    box-sizing: border-box;
}

body {
    font-family: 'Montserrat';
}

nav {
    background: #320911;
    height: 80px;
    width: 100%;
}

label.logo {
    color: #D3D3D3;
    font-size: 35px;
    line-height: 80px;
    padding: 0 100px;
    font-weight: bold;

}

nav ul {
    float: right;
    margin-right: 40px;
}

nav ul li {
    display: inline-block;
    line-height: 80px;
    margin: 0 5px;
}

nav ul li a {
    color: #D3D3D3;
    font-size: 17px;
    text-transform: uppercase;
    padding: 7px 13px;
    border-radius: 3px;
}

a.active,a:hover {
    background: #4f0c19;
    transition: .5s;
}
</style>

<!-- https://www.youtube.com/watch?v=oLgtucwjVII&ab_channel=CodingNepal -->
