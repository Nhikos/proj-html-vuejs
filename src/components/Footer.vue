<template>
  <div class="footer">
      <section class="section-left background">
          <div class="container">
            <h4>FIND OUR RESTAURANTS</h4>
            <Infobox
            v-for= "(info, index) in infos"
            :key= "index"
            :info="info"
            />
          </div>
          <div class="container">
            <h4>WORKING HOURS</h4>
            <div class="working">
                <div class="section">
                    <h5>MONDAY</h5>
                    <span>Kitchen Closed</span>
                </div>
                <div class="section">
                    <h5>TUESDAY UNTIL FRIDAY</h5>
                    <h6>9:00 - 22:00</h6>
                </div>
                <div class="section">
                    <h5>Saturday <span>*</span></h5>
                    <h6>Saturday 11am to midnight</h6>
                </div>
                <div class="section">
                    <h5>SUNDAY</h5>
                    <h6>9:00 - 22:00</h6>
                </div>
                <div class="section">
                    <span class="social">
                        <h5>Follow Us:</h5> 
                        <i class="fab fa-twitter"></i><i class="fab fa-facebook-f"></i><i class="fab fa-instagram"></i><i class="fab fa-linkedin-in"></i>
                    </span>
                </div>
            </div>
          </div>
          <div class="container">
              <h2>The don peppe crew first and foremost values an authentic, well baked slice of pizza.</h2>
          </div>
          <img class="logo-footer" src="../assets/img/footer-bottom-img.png" alt="">
      </section>
      <section class="section-right">

      </section>
  </div>
</template>

<script>
import Infobox from './Infobox.vue'
export default {
    name: "Footer",
    components: {
        Infobox
    },

    data: function() {
        return {
            infos: [
                {
                    via: "1614 E. Bell Rd #104.",
                    city: "Salerno, AZ 85022",
                    telephone: "(602)867-1010",
                },
                {
                    via: "204 E. Pizzetta Tommaso",
                    city: "Sorrento, AZ 85022",
                    telephone: "(358) 867-1010",
                },
                {
                    via: "Vale Puglia 54",
                    city: "Torre Del Greco, AZ 85022",
                    telephone: "(359) 867-1010",
                },
                {
                    via: "Corso Itali AA",
                    city: "Naples, AZ 85022",
                    telephone: "(989) 867-1010",
                },
            ],
        }
    }
}
</script>

<style scoped>
.footer {
    display: flex;
    height: 630px;
}

.background {
    background-color: #000000;
    background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23898989' fill-opacity='0.26' fill-rule='evenodd'/%3E%3C/svg%3E");
}

.section-left,
.section-right {
    width: 50%;
}

.section-left {
    display: flex;
    justify-content: flex-start;
    position: relative;
    padding: 125px 50px;
}

.section {
    margin: 20px 0;
}

h2 {
    color: white;
    text-transform: uppercase;
}

h4 {
    color: #af8a3a;
    font-size: 20px;
    margin-bottom: 20px;
}

h5 {
    color: #af8a3a;
    text-transform: uppercase;
}

h6 {
    color: #a7a7a7;
    font-size: 14px;
    margin-bottom: 20px;
}
span {
    color: red;
    font-size: 14px;
}

.social > h5 {
    display: inline-block;
    margin-right: 8px;
}

.social > i {
    color: white;
    font-size: 12px;
    margin-left: 10px;
    cursor: pointer;
}

.container {
    height: 458px;
    width: 252px;
}
.container:nth-of-type(3) {
    width: 230px;
}

.section-right {
    width: 50%;
    background-image: url(../assets/img/footer-img-1.jpg);
    background-size: contain;
}

.logo-footer {
    position: absolute;
    bottom: 0;
    right: 0;
    margin: 0px 50px 35px 0;
}
</style>