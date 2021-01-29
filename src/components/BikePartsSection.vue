<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col">

      <br>
      <h3>Frame</h3>
      <div class="bike-parts-container">
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
      </div>

      <br>
      <h3>Hub</h3>
      <div class="bike-parts-container">
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
      </div>

      <br>
      <h3>Rotor</h3>
      <div class="bike-parts-container">
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
        <div class="bike-parts-item">
        </div>
      </div>


      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      
    }
  }
}
</script>

<style lang="scss" scoped>
$font-family-Baloo2: Baloo 2, cursive;
$font-family-Raleway: Raleway, sans-serif;
$bg-white: #f2f2f2;

.bike-parts-container {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-gap: 10px;

  .bike-parts-item {
    background: $bg-white;
    height: 200px;
  }
}
h3 {
  font-family: $font-family-Raleway;
  font-size: 20px;
  font-weight: 300;
}

@media screen and (min-width: 768px) {
  .bike-parts-container { grid-template-columns: repeat(3, 1fr); }
}
@media screen and (min-width: 1024px) {
  .bike-parts-container { grid-template-columns: repeat(6, 1fr); }
}
</style>