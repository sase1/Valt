<template>
  <div>
    <Header />
    <!-- <header>
      <nav>
        <a href="#">
          <img
            src="../assets/Valtech-Logo-black@2x.png"
            alt=""
            class="logo--img"
          />
        </a>
        <input type="checkbox" id="click" />
        <label for="click" class="menu-btn">
          <i class="fas fa-bars"></i>
        </label>
        <ul>
          <li><a class="active" href="#">Section one</a></li>
          <li><a href="#">Section two</a></li>
          <li><a href="#">Section three</a></li>
          <li><a href="#">Section four</a></li>
        </ul>
        <div class="navbar--search">
          <input type="text" placeholder="Type text here..." />
          <button>SEARCH</button>
        </div>
      </nav>
    </header> -->
    <main>
      <SectionOne  />
      <!-- <section class="section--one">
        <div class="contact">
          <div class="contact--button">
            <a href="#">
              <button>CONTACT</button>
            </a>
            <p>Lorem ipsum dolor sit amet, consectetur</p>
          </div>
        </div>
      </section> -->
      <SectionTwo />

      <SectionThree />

      <!-- <section class="section--three">
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
      </section> -->
      <!-- <section class="section--four">
        <form action="">
          <div class="form--container">
              <div>
                <label class="form--label" for="">First Name</label><br />
                <input class="form--input" type="text" />
              </div>
                <div>
                <label class="form--label" for="">Last Name</label><br />
                <input class="form--input" type="text" />
              </div>
              <div>
                <label class="form--label" for="">Email address</label><br />
                <input class="form--input" type="text" />
              </div>
              <div>
                <label class="form--label" for="">Phone number</label><br />
                <input class="form--input" type="text" />
              </div>
              <div>
                <label class="form--label" for="">Your message</label><br />
                <textarea ></textarea>
              </div>
              <div>
                <button class="form--button">SEND</button>
              </div>
          </div>
        </form>
      </section> -->
      <SectionFour />
    </main>

    <!-- <footer>
      <div class="footer--logo">
        <img src="../assets/Valtech-Logo-black.png" alt="">
      </div>
     <div class="footer--menu">
        <div>
        <p>Footer Section Title</p>
        <ul>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
        </ul>
      </div>
        <div>
        <p>Footer Section Title</p>
        <ul>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
        </ul>
      </div>
        <div>
        <p>Footer Section Title</p>
        <ul>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
          <li><a href="#">Footer link</a></li>
        </ul>
      </div>
     </div>
    </footer> -->
    <Footer />
  </div>
</template>

<script>
import Header from "./Header";
import SectionOne from "./SectionOne";
import SectionTwo from "./SectionTwo";
import SectionThree from "./SectionThree";
import SectionFour from "./SectionFour";
import Footer from "./Footer";

export default {
  name: "HelloWorld",
  components: {
    Header,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    Footer,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
* {
  box-sizing: border-box;
}
/* nav {
  display: flex;
  height: 90px;
  width: 100%;
  align-items: center;
  justify-content: space-between;
  padding: 0 100px;
  flex-wrap: wrap;
}
.logo--img {
  height: 40px;
}
nav ul {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
}
nav ul li {
  margin: 0 15px;
}
nav ul li a {
  color: #707070;
  text-decoration: none;
  font-size: 18px;
  transition: all 0.3s ease;
}

.navbar--search input {
  height: 39px;
  width: 271px;
  border: 1px solid #195757;
  border-radius: 15px 0px 0px 15px;
  color: #707070;
  text-indent: 16px;
  font-size: 14px;
  outline: none;
}

.navbar--search button {
  background: #00e0ff;
  outline: none;
  color: #000000;
  font-size: 14px;
  border: none;
  height: 39px;
  padding: 0px 11px;
}

nav .menu-btn i {
  color: red;
  font-size: 22px;
  cursor: pointer;
  display: none;
}
input[type="checkbox"] {
  display: none;
}
@media (max-width: 1000px) {
  nav {
    padding: 0 40px 0 50px;
  }
}
@media (max-width: 920px) {
  nav .menu-btn i {
    display: block;
  }
  #click:checked ~ .menu-btn i:before {
    content: "\f00d";
  }
  nav ul {
    position: fixed;
    top: 80px;
    left: -100%;
    background: #111;
    height: 100vh;
    width: 100%;
    text-align: center;
    display: block;
    transition: all 0.3s ease;
  }
  #click:checked ~ ul {
    left: 0;
  }
  nav ul li {
    width: 100%;
    margin: 40px 0;
  }
  nav ul li a {
    width: 100%;
    margin-left: -100%;
    display: block;
    font-size: 20px;
    transition: 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }
  #click:checked ~ ul li a {
    margin-left: 0px;
  }
  nav ul li a.active,
  nav ul li a:hover {
    background: none;
    color: cyan;
  }
} */

/* NAVBAR CODE */
/* .section--one,
.section--four {
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
} */
/* SECTION ONE CODE */

/* .section--three {
  padding: 247px 0 83px 0;
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
} */
/* SECTION THREE CODE */

/* .section--four {
  background-image: url("../assets/Intersection_1.png");
  padding-top: 250px;
}

.form--container {
  width: 52%;
  margin: auto;
  background-color: rgba(255, 255, 255, 0.7);
  padding: 39px 48px;
  display: flex;
  justify-content: space-between;
  border-radius: 15px;
  flex-wrap: wrap;
} */

/* .form--right--block,
.form--left--block {
  width:290px;
} */

/* .form--container div {
  margin-bottom: 22px;
  width: 300px;
}

.form--container div:last-child{
  position: relative;
}

.form--input {
  width: 100%;
  height: 40px;
  border-radius: 15px;
  border: none;
  margin-top: 10px;
}

.form--label {
  padding-left: 8px;
}

.form--button {
  background-color: #000000;
  color: #ffffff;
  height: 50px;
  width: 200px;
  position: absolute;
  outline: none;
  right: 0;
  bottom: 0;
  border-radius: 15px;
  border: none;
  cursor: pointer;
}
textarea {
  border-radius: 15px;
  border: none;
  margin-top: 10px;
  width: 100%;
  height: 120px;
} */
/* SECTION FOUR CODE */

footer {
  /* display: flex; */
  /* justify-content: space-evenly; */
  margin-top: 65px;
}

footer ul li a {
  color: #000000;
}

footer ul li {
  margin-bottom: 3px;
}

footer ul {
  list-style: none;
  padding-left: 16px;
}

.footer--logo {
  width: 24%;
  float: left;
  text-align: center;
}

.footer--menu p {
  margin: 0;
}

.footer--menu {
  display: flex;
  width: 60%;
  justify-content: space-between;
}
</style>
