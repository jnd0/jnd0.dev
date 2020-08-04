<template>
  <div>

    <h1>Projects</h1>

    <div class="columns projects-grid">

      <a class="box" href="https://jnd0.dev">
        <h2>jnd0.dev</h2>
        <p>This website. </p>
      </a>

      <a class="box" href="https://blog.jnd0.dev">
        <h2>blog.jnd0.dev</h2>
        <p>My blog / open window to the world where I share my thoughts and learnings for someonelse to benefit from
          them.</p>
      </a>

      <a class="box" href="https://github.com/jnd0/tailwindcss-sepia-mode">
        <h2>tailwindcss-sepia-mode</h2>
        <p>Tailwind plugin that enables you to have the sepia attribute and be able to implement sepia-mode in the
          framework. </p>
      </a>

      <a class="box" href="https://jnd0.dev">
        <h2>More</h2>
        <p>comming soon</p>
      </a>
      <a class="box" href="https://jnd0.dev">
        <h2>Projects</h2>
        <p>comming soon</p>
      </a>
      <a class="box" href="https://jnd0.dev">
        <h2>Comming soon </h2>
        <p>comming soon</p>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "projects"
}
</script>

<style scoped>

h1{
  text-align: center;
  padding: 2rem;
}
.projects-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: flex-start;
  padding-top: 2rem;
}

.columns {
  margin-left: -.75rem;
  margin-right: -.75rem;
  margin-top: -.75rem;
}

.column {
  display: block;
  flex-basis: 0;
  flex-grow: 1;
  flex-shrink: 1;
  padding: .75rem;
}

.box {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 28%;
  border-radius: 6px;
  box-shadow: 0 2px 3px rgba(10, 10, 10, .1), 0 0 0 1px rgba(10, 10, 10, .1);
  padding: .75rem;
  transition: transform 200ms;
  height: 10rem;
  text-align: center;

}

.box:hover {
  box-shadow: 0 2px 10px rgba(10, 10, 10, .2), 0 0 0 1px rgba(10, 10, 10, .1);
  transform: scale(1.05);
  transition: all 200ms;
}

p {
  display: none;
}

.box:hover p {
  display: block;
}

.box:hover h2 {
  display: none;
}

a {
  text-decoration: none;
  display: block;

}


</style>
