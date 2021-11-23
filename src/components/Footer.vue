<template>
  <div>
    <footer>
      <div class="footer--logo">
        <img src="../assets/Valtech-Logo-black.png" alt="" />
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
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer {
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
