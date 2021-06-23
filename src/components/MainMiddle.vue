<template>
  <div class="main-middle">
        <div class="jumbotron-top">
            <div class="jumbo-text">
                <h1>go ahead and build your own pizza <br> we won't <br> judge!</h1>
            </div>
            <div class="jumbo-img-container">
                <div class="img1"></div>
                <div class="img2"></div>
                <div class="img3"></div>
            </div>
        </div>
        <div class="jumbotron-bot">
            <img src="../assets/img/h1-team-1a-700x700.jpg" alt="">
            <img src="../assets/img/h1-team-2a.jpg" alt="">
            <img src="../assets/img/h1-team-4a.jpg" alt="">
            <img src="../assets/img/h1-team-3a.jpg" alt="">
        </div>
        <div class="clients">
            <img src="../assets/img/h1-clients-img-4.png" alt="">
            <img src="../assets/img/h1-clients-img-3.png" alt="">
            <img src="../assets/img/h1-clients-img-1.png" alt="">
            <img src="../assets/img/h1-clients-img-2.png" alt="">
            <img src="../assets/img/h1-clients-img-5.png" alt="">
        </div>
        <div class="pizza-menu">
            <div class="pizza-menu-text">
                <h5>choose your flavor</h5>
                <h2>the best pizza menu in town</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam, necessitatibus! Dolorem rem nesciunt mollitia facere enim, repellat illo est.</p>
            </div>
            <div class="pizza-carousel">
                <div class="carta"></div>
                <div class="carta"></div>
                <div class="carta"></div>
                <div class="carta"></div>
                <div class="carta"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainMiddle"
}
</script>

<style scoped>

/* JUMBOTRON TOP */
.jumbotron-top {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    position: relative;
    height: 594px;
    width: 100%;
}

.jumbo-text {
    position: absolute;
    color: white;
    width: 360px;
    margin-left: 20%;
    font-size: 31px;
    text-transform: uppercase;
}
.jumbo-text > h1 {
    line-height: 67px;
}

.jumbo-img-container {
    height: 100%;
    width: 100%;
}
.img1 {
    height: 24%;
    background-image: url(../assets/img/h3-background-img.jpg);
    background-size: 90%;
    background-position-y: 143px;
    background-position-x: 50%;
}
.img2 {
    height: 52%;
    background-image: url(../assets/img/h3-background-img.jpg);
    background-size: 90%;
    background-position-y: 986px;
    background-position-x: 50%;
}
.img3 {
    height: 24%;
    background-image: url(../assets/img/h3-background-img.jpg);
    background-size: 90%;
    background-position-y: 432px;
    background-position-x: 50%;
}
/* /JUMBOTRON TOP */

/* JUMBOTRON BOT */
.jumbotron-bot {
    display: flex;
    height: 435px;
    width: 100%;
}
.jumbotron-bot > img {
    width: calc(100% / 4);
}
/* /JUMBOTRON BOT */
/* CLIENTS */
.clients {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 70%;
    height: 270px;
    margin: 0 auto;
    border: 1px solid blue;
}
.clients > img {
    height: 120px;
}
/* /CLIENTS */

.pizza-menu {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    align-items: center;
    height: 750px;
}

.pizza-menu-text {
    text-align: center;
    width: 30%;
    margin-top: 50px;
    border: 1px solid red;
}

.pizza-carousel {
    display: flex;
    flex-wrap: no-wrap;
    align-items: center;
    width: 100%;
    height: 50%;
    margin-bottom: 70px;
    border: 1px solid blue;
}

.carta {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 326px;
    width: 263px;
    margin: 58px;
    border: 1px solid green;
}
</style>