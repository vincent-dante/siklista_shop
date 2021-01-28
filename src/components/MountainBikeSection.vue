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

.product-container{ 
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 10px;

  .product-item{ 
    background: $bg-white;
    height: 300px;
  }
}
</style>