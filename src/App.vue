<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
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
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
