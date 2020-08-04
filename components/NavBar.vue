<template>
  <header class="header">
    <div class="home">
      <h3>
        <nuxt-link to="/"> jnd0.dev</nuxt-link>
      </h3>
    </div>
    <nav class="main-nav">
      <ul>
        <li>
          <a href="https://blog.jnd0.dev" target="_blank"> Blog</a>
        </li>
        <li>
          <nuxt-link to="/projects"> Personal projects</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/contact">Contact</nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>


<style scoped>

.header {
  display: flex;
  align-items: center;
  justify-content: space-around;
  padding: 10px;
}

.main-nav ul {

}

.main-nav li {
  display: inline;
}

.main-nav a {
  padding-left: 0.5em;
}


</style>
