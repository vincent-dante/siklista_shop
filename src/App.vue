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
<!--         <form class="d-flex" @submit.prevent="">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form> -->
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
<<<<<<< HEAD
          <p>Hello</p>
=======
          <h4>sss</h4>
>>>>>>> 12e144a96fca8c057b3df89c485e2f40ff0ff723
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
            <p class="footer-logo">Siklista</p>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <div class="footer-links-container">
              <p>Product</p>
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
$bg-white: #f2f2f2;

.homepage-header {
  background: $bg-white;
  height: 500px;
}
.product-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 10px;

  .product-item {
    background: $bg-white;
    height: 300px;
  }
}
h2 {
  font-family: $font-family-Caveat;
  font-size: 32px;
}
.brand-style {
  font-family: $font-family-Caveat;
  font-size: 35px;
}
.main-footer {
  background: $bg-white;
  padding-top: 30px;

  .footer-logo {
    font-family: $font-family-Caveat;
    font-size: 32px;
    text-align: center;
  }
  .footer-links-container {
    display: flexbox;
    
  }

}

</style>
