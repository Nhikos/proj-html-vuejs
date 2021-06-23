<template>
  <div class="main">
      <div class="main-top">
          <section class="main-section-top">
            <img src="../assets/img/h3-img-1.jpg" alt="">
            <img src="../assets/img/h3-img-2.jpg" alt="">
            <img src="../assets/img/h3-img-3.jpg" alt="">
            <img src="../assets/img/h3-img-4.jpg" alt="">
          </section>
          <section class="main-section-mid">
              <div class="prev ball">
                  <span>prev</span>
              </div>
              <div class="cit-container">
                <i class="fas fa-quote-left"></i>
                <h3>"FORGET THE TRENDY PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h3>
                <span class="location">WASHINGTON POST 2018</span>
                <div class="circles">
                    <span class="circle"></span>
                    <span class="circle"></span>
                    <span class="circle"></span>
                </div>
              </div>
              <div class="next ball">
                  <span>next</span>
              </div>
          </section>
          <section class="main-section-bot">
            <section class="main-section-bot_left"></section>
            <section class="main-section-bot_right">
                <div class="offers_container">
                        <h2>SPECIALS*</h2>
                        <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio, deleniti!</span>
                    <div class="offer-description">
                        <div class="offer-price">
                            <h3>$10</h3>
                        </div>
                        <div class="offer-type">
                            <h3>COMBO PICCOLO</h3>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, est.</span>
                        </div>
                    </div>
                    <div class="offer-description">
                        <div class="offer-price">
                            <h3>$20</h3>
                        </div>
                        <div class="offer-type">
                            <h3>COMBO MEZZO</h3>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, est.</span>
                        </div>
                    </div>
                    <div class="offer-description">
                        <div class="offer-price">
                            <h3>$30</h3>
                        </div>
                        <div class="offer-type">
                            <h3>COMBO GRANDE</h3>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, est.</span>
                        </div>
                    </div>
                </div>
            </section>
          </section>
      </div>
  </div>
</template>

<script>
export default {
    name: "MainMiddle"
}
</script>

<style scoped>
/* COMMON */
.main {
    margin-top: 6px;
}
/* /COMMON */

/* MAIN TOP */
/* main-SECTION-TOP */
.main-section-top {
    display: flex;
    justify-content: space-between;
}
.main-section-top img {
    display: flex;
    width: calc(100% / 4 - 6px)
}
/* /SECTION TOP */

/* SECTION MIDDLE */
.main-section-mid {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 316px;
    margin: 5px 0;
    background-image: url(../assets/img/h3-testimonials-bckgrnd.jpg);
    background-position: center;
}

.fa-quote-left {
    font-size: 45px;
    margin-bottom: 15px;
}

.main-section-mid h3 {
    text-align: center;
    margin-bottom: 10px
}

.location {
    color: red;
    margin-bottom: 15px;
    font-size: 10px;
}


.circle {
    display: inline-block;
    height: 5px;
    width: 5px;
    padding: 3px 3px;
    margin: 10px 3px;
    border-radius: 50%;
    background-color: #b7903c;
}


.cit-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 30%;
}

.fa-quote-left {
    color: #b7903c;
}

.prev {
    color: red;
    writing-mode: vertical-rl;
}
.next {
    color: red;
    writing-mode: vertical-rl;
    transform:rotateZ(180deg)
}
.ball {
    padding: 18px 10px;
    background-color: white;
    border-top-right-radius: 50%;
    border-bottom-right-radius: 50%;
}
/* /SECTION MIDDLE */

/* SECTION BOTTOM */
.main-section-bot {
    display: flex;
    height: 770px;
    width: 100%;
    margin-bottom: 5px;
}

/* SECTION BOTTOM-LEFT */
.main-section-bot_left {
    width: 50%;
    background-image:url(../assets/img/h1-img-4.jpg);
    background-size: cover;
}
/* /SECTION BOTTOM-LEFT */

/* SECTION BOTTOM-RIGHT */
.main-section-bot_right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 50%;
}

.offers_container {
    width: 40%;
}

.offers_container span {
    color: #777777;
}

.offer-description {
    display: flex;
    margin: 10px 0;
    justify-content: space-between;
}
.offer-description  h3 {
    margin-bottom: 6px;
}

.offer-price {
    color: #b14e38;
}

.offer-type {
    width: 85%;
}
/* /SECTION BOTTOM-RIGHT */
/* /SECTION BOTTOM */
</style>