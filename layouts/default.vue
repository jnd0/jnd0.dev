<template>
  <div class="layout">
    <NavBar/>
    <main>
      <nuxt/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import NavBar from '../components/NavBar';
import Footer from "../components/Footer";

export default {
  components: {
    Footer,
    NavBar
  }
}

</script>

<style>

body, html {
  padding: 0;
  margin: 0;
  background: #f8f8f8;
  font-family: 'Life Savers', cursive;

}

.layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  width: 100%;
}

main {
  flex: 1;
}

*,
*:before,
*:after {
  margin: 0;
}


</style>
