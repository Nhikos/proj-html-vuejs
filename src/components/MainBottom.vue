<template>
  <div class="main-bottom">
      <section class="section-top">
          <div class="pizza-deals-container">
                <div class="pizza-deals">
                    <span>made with love</span>
                    <h3>delish pizza deals</h3>
                    <div class="deal-container">
                        <div class="date">
                            <h2>02</h2>
                            <h3>nov</h3>
                        </div>
                        <div class="location">
                            <h3>tradition neopolitan pies in kyioto pizza mercato</h3>
                            <span>204 E. Piazzetta Tommaso</span>
                        </div>
                    </div>
                    <div class="deal-container">
                        <div class="date">
                            <h2>03</h2>
                            <h3>nov</h3>
                        </div>
                        <div class="location">
                            <h3>tradition neopolitan pies in kyioto pizza mercato</h3>
                            <span>204 E. Piazzetta Tommaso</span>
                        </div>
                    </div>
                    <div class="deal-container">
                        <div class="date">
                            <h2>05</h2>
                            <h3>nov</h3>
                        </div>
                        <div class="location">
                            <h3>tradition neopolitan pies in kyioto pizza mercato</h3>
                            <span>204 E. Piazzetta Tommaso</span>
                        </div>
                    </div>
                </div>
            </div>
          <div class="comic">
              <img src="../assets/img/h3-img-5a.jpg" alt="">
          </div>
      </section>
      <section class="section-bot">
          <div class="order-container">
              <div class="order-persons">
                <select name="cars" id="cars">
                    <option value="1">1 person</option>
                    <option value="2">2 persons</option>
                    <option value="3">3 persons</option>
                    <option value="4">4 persons</option>
                </select>
                <i class="fas fa-user-friends"></i>
              </div>
              <span>FOR</span>
              <div class="order-date">
                <form action="/action_page.php">
                <input type="date" id="birthday" name="birthday">
                </form>
              </div>
              <span>AT</span>
              <div class="order-hour">
                <input type="time">
              </div>
              <button>book a table</button>
          </div>
      </section>
  </div>
</template>

<script>
export default {
    name: "MainBottom"
}
</script>

<style scope>
.main-bottom {
    width: 100%;
}
.section-top {
    display: flex;
    height: 590px;
    margin-bottom: 10px;
}
.pizza-deals-container {
    display: flex;
    justify-content: center;
    color: white;
    height: 95%;
    width: 50%;
    padding: 20px 0;
    background-color: black;
    text-transform: uppercase;
}
.pizza-deals {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 41%;
}
.pizza-deals span {
    color: #ab4027;
    font-size: 10px;
}
.deal-container {
    display: flex;
    padding: 25px 0;
}

.deal-container:nth-of-type(2) {
    border-top: 1px dotted orange;
    border-bottom: 1px dotted orange;
}
.date {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    margin-right: 50px;
}
.date h2 {
    color: #ab4027;
    font-size: 40px;
    line-height: 43px;
}
.date  h3 {
    color: white;
    font: 15px;
}
/* .location {

} */

.comic {
    height: 100%;
    width: 50%;
}
.comic img {
    height: 100%;
    width: 100%;
}

.section-bot {
    display: flex;
    justify-content: center;
    background-image: url(../assets/img/h3-background-img-3.jpg);
    margin-bottom: 10px;
}
.order-container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;
    height: 200px;
    width: 700px;
}

input {
    padding: 10px;
    cursor: pointer;
}

select {
    width: 170px;
    padding: 10px;
    cursor: pointer;
}

.fa-user-friends {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: 25px;
    color: #ad893a;
    margin-left: 5px;
}

.order-persons {
    position: relative;
}

button {
    color: white;
    font-size: 10px;
    padding: 14px 22px;
    margin-left: 25px;
    background-color: #d2401e;
    text-transform: uppercase;
    border: none;
    cursor: pointer;
}
</style>