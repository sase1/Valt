<template>
  <div>
    <header>
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
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

nav {
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
  cursor: pointer;
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
}
</style>
