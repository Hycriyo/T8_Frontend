<template>
  <header>
  </header>
  <nav class="navbar navbar-expand-sm navbar-light bg-light">
    <a class="navbar-brand" href="/"><img src="https://picsum.photos/seed/picsum/75/75" alt="Random Logo"></a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item active">
        <router-link class="nav-link sr-only" to="/">Home</router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/lps">lps</router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/checker">checker</router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/nieuws">nieuws</router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/over_ons">over_ons</router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/contact">contact</router-link>
        </li>
      </ul>
    </div>
  </nav>
  <router-view/>
  <footer class="d-flex justify-content-sm-around justify-content-sm-between">
    <div>
        <h4>
            Snelle links:
        </h4>
        <a href="..//index.html">
            <h5>
                Home
            </h5>
        </a>
        <a href="../pages/lps.html">
            <h5>
                LP's
            </h5>
        </a>
        <a href="../pages/checker.html">
            <h5>
                Checker
            </h5>
        </a>
        <a href="../pages/nieuws.html">
            <h5>
                Nieuws
            </h5>
        </a>
        <a href="../pages/over_ons.html">
            <h5>
                Over ons
            </h5>
        </a>
        <a href="../pages/contact.html">
            <h5>
                Contact
            </h5>
        </a>
    </div>
    <div>
        <h5>
            &copy; Justin van Bruchem
        </h5>
    </div>
  </footer>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  /* color: #06488a; */
}

nav a.router-link-exact-active {
  color: #42b983;
}

@font-face {
    font-family: moupali;
    src: url(/src/assets/fonts/Moulpali-Regular.ttf);
}

h5,p,a,label,li
{
    color: #FFFFFF;
    font-family: moupali;
    line-height: 20px;
    font-size: 16px;
}

h1,h2
{
    color: #a88b17;
    font-family: moupali;
    font-size: 32px
}

h3,h4
{
    color: #FFF201;
    font-family: moupali;
    font-size: 20px;
    line-height: 10px;
}


html
{
    /* hoogte forceren naar 100% zodat absolute elementen bij het scrollen niet gaan zweven*/
    height: 100%;
}

/* algemene fontfamily voor de body bepaald, positie naar relatief, de minimale hoogte naar 100vh forceren,
de margin weghalen en een achtergrond plaatje toevoegen */
body
{
    background-color: #3A4750;
}

header
{
  background-image: url(/src/assets/images/vinyl_logo_banner.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  height: 15vh;
  border-bottom-style: solid;
  border-color: #F64E8B;
} 

hr
{
    color:#F64E8B;
    border-top: 2px solid;
    border-color: #F64E8B;
    margin-top: 0;
    margin-bottom: 0;
}

footer
{
    background-color: #3A4750;
    margin-top: auto;
    border-top-style: solid;
    border-color: #F64E8B;
    padding: 16px;
}

footer h4
{
    margin-top: 4px;
    margin-bottom: 20px;
}

footer h5
{
    margin: 4px;
}

footer a
{
    text-decoration: none;
}

</style>
