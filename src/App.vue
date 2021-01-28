<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand brand-style" href="#">Siklista Shop</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Product</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">About</a>
          </li>
        </ul>
        <form class="d-flex" @submit.prevent="">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
  
  <br>

  <main>
    <div class="container">
      <div class="row">
        <div class="col">
          
          <br>
          <h2>Mountain Bike</h2>
          <MountainBikeSection></MountainBikeSection> 
          <br>
          <br>
          <br>

          <h2>Mountain Bike Parts</h2>
          <BikePartSection></BikePartSection> 

        </div>
      </div>
    </div>
  </main>

  <br>

</template>

<script>
import MountainBikeSection from './components/MountainBikeSection';
import BikePartSection from './components/BikePartsSection';

export default {
  name: 'App',
  data(){
    return {
      
    }
  },
  components: {
    MountainBikeSection,
    BikePartSection,
  }
}
</script>

<style>
.homepage-header {
  background: #f2f2f2;
  height: 500px;
}
.product-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 10px;
}
.product-item {
  background: #f2f2f2;
  height: 300px;
}
.bike-parts-container {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-gap: 10px;
}
.bike-parts-item {
  background: #f2f2f2;
  height: 200px;
}
h2 {
  font-family: 'Caveat', cursive;
  font-size: 32px;
}
h3 {
  font-family: 'Baloo 2', cursive;
  font-size: 20px;
}
.brand-style {
  font-family: 'Caveat', cursive;
  font-size: 35px;
}
</style>
