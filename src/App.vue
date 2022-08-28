<script setup>
import Homepage from "./components/Homepage.vue";
//import Test from "./components/test.vue";
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-light cust-bg-nav shadow fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="./assets/Organics-skincare-logo-transp.png" height="90" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item px-4">
            <a class="nav-link active" aria-current="page" href="#home">Home</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#about">About</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#jenis-kulit">Jenis Kulit</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#product">Product</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#artikel">Artikel</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <main>
    <Test />
    <Homepage />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
