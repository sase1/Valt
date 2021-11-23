<template>
  <div>
    <section class="section--four">
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
            <textarea></textarea>
          </div>
          <div>
            <button class="form--button">SEND</button>
          </div>
        </div>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  name: "SectionFour",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.section--four {
  background-image: url("../assets/Intersection_1.png");
  /* height: 800px; */
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center ;
  /* padding-top: 100px; */
  /* padding-bottom: 65px; */
  padding: 50px;
}

.form--container {
  width: 53%;
  margin: auto;
  background-color: rgba(255, 255, 255, 0.7);
  padding: 39px 48px;
  display: flex;
  justify-content: space-between;
  border-radius: 15px;
  flex-wrap: wrap;
}

.form--container div {
  margin-bottom: 22px;
  width: 300px;
}

.form--container div:last-child {
  position: relative;
}

.form--input,
textarea {
  width: 100%;
  height: 40px;
  border-radius: 15px;
  border: none;
  margin-top: 10px;
  outline: none;
  text-indent: 12px;
}

textarea {
  height: 120px;
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
  bottom: 4px;
  border-radius: 15px;
  border: none;
  cursor: pointer;
}
</style>
