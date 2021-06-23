<template>
<div class="background">
  <div class="header">
   <div class="nav">
       <button> order online </button>
       <div class="actions">
        <ul>
            <li
            v-for= "(leftAction, index) in leftActions"
            :key = "index">
            <img class= "svg" :src="leftAction.image" alt="">
            {{ leftAction.name }}
            </li>
        </ul>
        <img src="../assets/img/h5-logo-divided-header.png" alt="">
        <ul>
            <li
            v-for= "(rightAction, index) in rightActions"
            :key = "index">
            {{ rightAction.name }}
            </li>
        </ul>
       </div>
       <div class="shop-action">
        <i class="fas fa-motorcycle"></i><a href="#">CART</a>
        <i class="fas fa-search"></i><a href="#">SEARCH</a>
       </div>
   </div>
   <img src="../assets/img/h3-rev-img-6.png" alt="">
  </div>
</div>
</template>

<script>
export default {
  name: 'Header',
  data:function() {
    return {
        leftActions: [
            {
                name: "HOME",
                link: "",
                image: require("../assets/svg/svg-0.svg")
            },
            {
                name: "PAGES",
                link: "",
                image: ""
            },
            {
                name: "MENU",
                link: "",
                image: ""
            }
        ],
        rightActions: [
            {
                name: "EVENT",
                link: "",
                image: ""
            },
            {
                name: "BLOG",
                link: "",
                image: ""
            },
            {
                name: "LANDING",
                link: "",
                image: ""
            }
        ]
    }
  }
}
</script>

<style scoped>
.background {
    background-color: #000000;
    background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23898989' fill-opacity='0.26' fill-rule='evenodd'/%3E%3C/svg%3E");
}

.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 422px;
    background-image: url(../assets/img/h3-rev-img-5.png);
    background-size: 41%;
    background-repeat: no-repeat;
    background-position: center;
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 25%;
    width: 75%;
}

.header > img {
    width: 12%;
}

a {
    font-size: 12px;
    text-decoration: none;
    color: white;
    cursor: pointer;
}
.actions{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-left: -50px;
}
.actions  .svg {
    display: inline-block;
    width: 13px;
    margin: 3px
}
.actions > a {
    margin-right: 25px;
    cursor: pointer;
}
.actions > img {
    width: 100px;
    margin: 0 20px;
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
    cursor: pointer;
}

ul {
    display: flex;
    color: white;
    font-size: 12px;
    margin: 0 15px;
    list-style: none;
}

i {
    color: white;
    font-size: 10px;
    margin: 0px 5px;
    cursor: pointer;
}

li {
    margin: 0 10px;
    cursor: pointer;
}
button {
    color: white;
    font-size: 12px;
    padding: 10px 20px;
    margin-left: 0px;
    background-color: #d2401e;
    text-transform: uppercase;
    border: none;
    cursor: pointer;
}

</style>