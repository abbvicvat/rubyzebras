<template>
  <div class="flex-col pt-24">
    <div id="input-div-div">
      <div class="input-div">
        <input id="email" type="text" placeholder="Email" class="input">
        <hr class="line">
      </div>
      <div class="input-div">
        <input id="password" type="password" placeholder="Password" class="input">
        <hr class="line">
      </div>
      <button class="button bg-green-500 mt-12" @click="submit">
        Log In
      </button>
    </div>
  </div>
</template>

<script>
import data from '../db.json'

export default {
  async fetch() { console.log("users:", this.users); },

  data() {
    return {
      users: data.customers
    }
  },

  methods: {
    submit() {
      let email = document.getElementById("email").value;
      let password = document.getElementById("password").value;
      
      let valid = false;
      console.log("email: ", email);
      console.log("password: ", password);
      for (let i = 0; i < this.users.length; ++i) {
        if (email == this.users[i].email && password == this.users[i].password) {
          valid = true;
          alert("Log in successful")
          localStorage.setItem("id", this.users[i].id); 
          localStorage.setItem("name", this.users[i].name);
          console.log(localStorage.getItem("id"));
          console.log(localStorage.getItem("name"));
          break;
        }
      }

      if (!valid) alert("Wrong email or password")
    }
  }
}
</script>

<style scoped>
  #input-div-div {
    display: flex;
    flex-direction: column;

    align-items: center;
  }
  .input-div {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .input {
    margin-top: 20px;
    margin-bottom: 10px;
    padding-left: 10px;
    width: 25vw;
    height: 4vh;
  }
  .line {
    width: 30vw;
    border-width: 1px;
    border-color: #707070;
  }
  
  .button {
    border: none;
    color: white;
    padding: 8px 150px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
  }

  .button:hover {
    background-color: #059669;
  }

  .button:active {
    background-color: #059669;
    box-shadow: 0 5px #666;
    transform: translateY(1px);
  }
</style>
