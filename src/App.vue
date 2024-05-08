<template>
  <header>
  </header>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item active">
            <router-link class="nav-link sr-only" to="/">Home</router-link>
        </li>
        <li class="nav-item">
            <router-link class="nav-link" to="/lps">Lp's</router-link>
        </li>
        <li class="nav-item">
            <router-link class="nav-link" to="/checker">Checker</router-link>
        </li>
        <li class="nav-item">
            <router-link class="nav-link" to="/nieuws">Nieuws</router-link>
        </li>
        <li class="nav-item">
            <router-link class="nav-link" to="/over_ons">Over ons</router-link>
        </li>
        <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact</router-link>
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

<style lang="less">
@achtergrondkleur: #3A4750;
@accentkleur: #F64E8B;
@textkleur: #FFFFFF;
@hoofdtitel: #F6C90E;
@subtitel: #FFF201;

@font-face 
{
    font-family: moupali;
    src: url(/src/assets/fonts/Moulpali-Regular.ttf);
}
#app {
    font-family: moupali;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    background-color: @achtergrondkleur;
    display:flex;
    flex-direction: column;
    // position: relative;
    min-height:100vh;
}

*
{
    /* boxsizing zorgt ervoor dat de border en inhoud totaal de hoogte / breedte zijn ipv alleen de inhoud */
    box-sizing: border-box;
    /* zorgt ervoor dat het scrollen smooth gaat en niet in een keer verspringt */
    scroll-behavior: smooth;   
     
}



h5,p,a,label,li
{
    color: @textkleur !important;
    line-height: 20px;
    font-size: 16px !important;
}

h1,h2
{
    color: @hoofdtitel !important;
    font-size: 32px !important;
}

h3,h4
{
    color: @subtitel !important;
    font-size: 20px !important;
    line-height: 10px;
}


html
{
    /* hoogte forceren naar 100% zodat absolute elementen bij het scrollen niet gaan zweven*/
    height: 100%;
}

/* algemene fontfamily voor de body bepaald, positie naar relatief, de minimale hoogte naar 100vh forceren,
de margin weghalen en een achtergrond plaatje toevoegen */

header
{
    display: flex;
    background-image: url(/src/assets/images/vinyl_logo_banner.png);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center center;
    justify-content: space-around;
    height: 15vh;
    border-bottom-style: solid;
    border-color: @accentkleur;
} 

hr
{
    color:@accentkleur;
    border-top: 2px solid;
    border-color: @accentkleur;
    margin-top: 0;
    margin-bottom: 0;
}

header img
{
    max-height: 100%;
    max-width: 100%;
}

nav 
{
    padding: 30px;
    height: 64px;
    border-top-style: solid;
    border-color: @accentkleur;
    border-width: 4px;
}

nav a 
{
  font-weight: bold;
}

.nav-item .router-link-active 
{
  color: @hoofdtitel !important;
}

.nav-item:hover
{
    background-color: @accentkleur !important;
}

.nav-item
{    
    max-height: calc(100vh / 6);
    width: 100%;
    text-align: center;
}

.nav-link
{
    width: 100%;
    height: 100%;

}

.navbar-nav
{
    background-color: @achtergrondkleur !important;
}

main>h2
{
    text-align: center;
}

footer
{
    background-color: @achtergrondkleur;
    display: flex;
    justify-content: space-between;
    margin-top: auto;
    border-top-style: solid;
    border-color: @accentkleur;
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

@media screen and (orientation: landscape) and (max-height: 380px)
{
    nav>div
    {
        height: 48px;
    }
}


@media screen and (min-width: 992px)
{
    .navbar-expand-lg .navbar-nav 
    {
        width: 100%;
    }
    h5,p,a,label,li
    {
        font-size: 18px;
    }

    h1,h2
    {
        font-size: 46px
    }

    h3,h4
    {
        font-size: 22px;
        line-height: 2px;
    }

    nav
    {
        margin-top: 16px;
        width: 100%;
        border-bottom: solid 4px @accentkleur;
    }

    #hamburgerButton
    {
        display: none;
    }

    footer
    {
        justify-content: center;
    }

    footer>div
    {
        margin-left: 32px;
        margin-right: 32px;
    }
}
</style>
