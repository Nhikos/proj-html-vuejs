<template>
  <div class="card">
      <img 
      :class="pizza.sold == false ? 'sold' : '' "
      :src="pizza.image" alt="">
      <h3>{{pizza.name}}</h3>
      <h4>{{pizza.price}}</h4>
  </div>
</template>

<script>
export default {
    name: "Card",
    props: {
        pizza: Object,
    }
}
</script>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;
    height: 326px;
    width: 263px;
    margin: 0 58px;
    cursor: pointer;
}
.card h3 {
    color: #B7903C;
    font-size: 14px;
}

.card h4 {
    color: #D2401E;
    font-size: 13px;
}
img {
    height: 190px;
    margin-bottom: 10px;
}
.sold {
    position: relative;
}
.sold::after {
    content: "";
    position: absolute;
    height: 10px;
    width: 10px;
    background-color: brown;
    border-radius: 50%;
}

</style>