<template>
  <div>
    <section class="section--one">
      <div class="contact">
        <div class="contact--button">
          <a href="#">
            <button>CONTACT</button>
          </a>
          <p>Lorem ipsum dolor sit amet, consectetur</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "SectionOne",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.section--one {
  background-image: url("../assets/Intersection_2.png");
  height: 800px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.contact {
  height: 253px;
  background-color: rgba(255, 255, 255, 0.8);
  position: relative;
  top: 300px;
}

.contact--button {
  text-align: center;
  position: relative;
  top: 101px;
}

.contact--button p {
  font-size: 12px;
}

.contact--button button {
  background: #221f1f;
  box-shadow: 0px 8px 0px #00000033;
  border-radius: 30px;
  width: 280px;
  height: 60px;
  font-size: 18px;
  outline: none;
  color: #ffffff;
  cursor: pointer;
}
</style>
