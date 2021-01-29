<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col">
        <div class="product-container">
          <div class="product-item">
          </div>
          <div class="product-item">
          </div>
          <div class="product-item">
          </div>
          <div class="product-item">
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
$bg-white: #f2f2f2;

.product-container { 
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-gap: 10px;

  .product-item{ 
    background: $bg-white;
    height: 300px;
  }
}

@media screen and (min-width: 768px) {
  .product-container { grid-template-columns: repeat(2, 1fr); }
}
@media screen and (min-width: 1024px) {
  .product-container { grid-template-columns: repeat(4, 1fr); }
}
</style>