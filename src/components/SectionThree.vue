<template>
  <div>
    <section class="section--three">
      <div class="whole--card--content">
        <div class="card-img card-img-1"></div>
        <div class="card--text--content">
          <p class="title">Teaser title</p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc enim
            ligula, auctor rhoncus massa non, congue dignissim sapien.
            Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
            posuere cubilia curae
          </p>
          <button>Read more</button>
        </div>
      </div>
      <div class="whole--card--content">
        <div class="card-img card-img-3"></div>
        <div class="card--text--content">
          <p class="title">Teaser title</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
          <button>Read more</button>
        </div>
      </div>
      <div class="whole--card--content">
        <div class="card-img card-img-2"></div>
        <div class="card--text--content">
          <p class="title">Teaser title</p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc enim
            ligula, auctor rhoncus massa non, congue dignissim sapien.
          </p>
          <button>Read more</button>
        </div>
      </div>
      <div class="whole--card--content">
        <div class="card-img card-img-4"></div>
        <div class="card--text--content">
          <p class="title">Teaser title</p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc enim
            ligula, auctor rhoncus massa non, congue dignissim sapien.
            Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
            posuere cubilia curae Vestibulum ante ipsum…
          </p>
          <button>Read more</button>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "SectionThree",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.section--three {
  padding: 150px 0 83px 0;
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  width: 100%;
  margin: auto;
}

.whole--card--content {
  width: 536px;
  margin-bottom: 50px;
}

.card--text--content {
  padding: 30px;
  box-shadow: 0px 8px 5px #00000029;
  border-radius: 0px 0px 15px 15px;
  min-height: 250px;
  height: auto;
  position: relative;
}

.card--text--content button {
  float: right;
  width: 150px;
  height: 40px;
  background-color: #000000;
  color: #ffffff;
  border-radius: 10px;
  border: none;
  position: absolute;
  right: 40px;
  bottom: 20px;
  cursor: pointer;
}
div.card-img {
  height: 260px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: top;
}
.card--text--content p {
  font-size: 16px;
}

.card--text--content p.title {
  font-size: 32px;
  margin-top: 0;
}

div.card-img-1 {
  background-image: url("../assets/large-emerging-technologies.png");
}
div.card-img-2 {
  background-image: url("../assets/large-emerging-technologies3.png");
}
div.card-img-3 {
  background-image: url("../assets/large-emerging-technologies2.png");
}
div.card-img-4 {
  background-image: url("../assets/large-emerging-technologies4.png");
}
</style>
