<template>
  <div class="header">
   <div class="nav">
       <button> order online </button>
       <div class="actions">
        <img class="svg" src="../assets/svg/svg-0.svg" alt=""><a href="#">lorem</a>
        <a href="#">lorem</a>
        <a href="#">lorem</a>
        <img src="../assets/img/h5-logo-divided-header.png" alt="">
        <a href="#">lorem</a>
        <a href="#">lorem</a>
        <a href="#">lorem</a>
       </div>
       <div class="shop-action">
        <img class="svg" src="../assets/svg/svg-1.svg" alt=""><a href="#">lorem</a>
        <img class="svg" src="../assets/svg/svg-11.svg" alt=""><a href="#">lorem</a>
       </div>
   </div>
   <img src="../assets/img/h3-rev-img-6.png" alt="">
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 422px;
    background-image: url(../assets/img/h3-rev-img-5.png);
    background-size: 41%;
    background-repeat: no-repeat;
    background-position: center;
    background-color: black;
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 25%;
    width: 60%;
    border: 1px solid blue;
}

.header > img {
    width: 16%;
}

a {
    font-size: 12px;
    text-decoration: none;
    color: white;
}
.actions{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.actions > .svg {
    width: 13px;
    margin: 3px
}
.actions > a {
    margin-right: 25px;
}
.actions > img {
    width: 100px;
    margin-right: 26px;
}

.shop-action {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.shop-action > img {
    height: 20px;
}
.shop-action > a {
    margin-right: 10px;
}


button {
    color: white;
    font-size: 12px;
    padding: 10px 20px;
    background-color: orangered;
    text-transform: uppercase;
    border: none;
}

</style>