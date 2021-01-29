<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand brand-style" href="#">Siklista Shop</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto mb-2 mb-lg-0 nav-style">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">Products</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">About</a>
          </li>
        </ul>
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

  <footer>
    <div class="main-footer">
      <div class="container">
        <div class="row">
          <div class="col">
            <p class="footer-logo">Siklista Shop</p>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <div class="footer-links-container">
              <p>Products</p>
              <p>About</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
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

<style lang="scss" scoped>
$font-family-Caveat: Caveat, cursive;
$font-family-Baloo2: Baloo 2, cursive;
$font-family-Raleway: Raleway, sans-serif;
$bg-white: #f2f2f2;

.homepage-header {
  background: $bg-white;
  height: 500px;
}
.nav-style {
  font-family: $font-family-Raleway;
  font-weight: 300;
}
h2 {
  font-family: $font-family-Raleway;
  font-size: 24px;
}
.brand-style {
  font-family: $font-family-Caveat;
  font-size: 35px;
}
.main-footer {
  padding-top: 30px;

  .footer-logo {
    font-family: $font-family-Caveat;
    font-size: 32px;
    text-align: center;
  }
  .footer-links-container {
    display: flex;
    justify-content: center;
    padding: 0 0 40px 0;

    p {
      font-family: $font-family-Raleway;
      padding: 0 20px;
      font-weight: 300;
    }
  }
}


</style>
