<template>
  <div>
    <section class="section--two">
      <input
        type="text"
        v-model="search"
        placeholder="Filter users by name..."
        @keyup='charCount()'
      />
      <span>{{ totalCharacter }} characters</span>
      <button @click="sort">Sort users by age</button>
      <table>
        <thead>
          <tr>
            <th>ID</th>
            <th>Image</th>
            <th>First Name</th>
            <th>Last Name</th>
            <th>Age</th>
            <th v-if="this.userInfo">Profession</th>
          </tr>
        </thead>
        <tbody v-if="this.totalCharacter >= 3">
          <tr v-for="(user, index) in filteredList" :key="index" @click="showExtraUserInfo">
            <td>{{ user.id }}aaa</td>
            <td><img :src="user.img" alt="image :)" /></td>
            <td>{{ user.firstname }}</td>
            <td>{{ user.lastname }}</td>
            <td>{{ user.age }}</td>
            <td>{{ user.profession }}</td>
          </tr>
        </tbody>
         <tbody v-else>
          <tr v-for="(user, index) in users" :key="index"  @click="showExtraUserInfo">
            <td>{{ user.id }}bbb</td>
            <td><img :src="user.img" alt="image :)" /></td>
            <td>{{ user.firstname }}</td>
            <td>{{ user.lastname }}</td>
            <td>{{ user.age }}</td>
            <td>{{ user.profession }}</td>
          </tr>
        </tbody>
      </table>
    </section>
  </div>
</template>

<script>
export default {
  name: "SectionTwo",
  data() {
    return {
      search: "",
      users: [],
      totalCharacter: 0,
      userInfo: false
    };
  },

  computed: {
    filteredList() {
      return this.users.filter((post) => {
        return post.firstname.toLowerCase().includes(this.search.toLowerCase());
      });
    },
  },
  methods: {
    sort() {
      return this.users.sort((a, b) => {
        return a.age - b.age;
      });
    },
      charCount(){
         this.totalCharacter = this.search.length;
       },
       showExtraUserInfo(){
         this.userInfo = true;
       }
  },
  mounted() {
    fetch("http://localhost:3000/users")
      .then((res) => res.json())
      .then((data) => (this.users = data))
      .catch((err) => console.log(err.message));
    console.log(this.users);
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
table {
  width: 750px;
  border-collapse: collapse;
  margin: 50px auto;
}

/* Zebra striping */
tr:nth-of-type(odd) {
  background: #eee;
}

th {
  background: #3498db;
  color: white;
  font-weight: bold;
}

td,
th {
  padding: 10px;
  border: 1px solid #ccc;
  text-align: left;
  font-size: 18px;
}
</style>
