<template>
  <div class="flex-col pt-24">
    <div id="input-div-div">
      <div class="input-div">
        <input id="email" type="text" placeholder="Email" class="input">
        <hr class="line">
      </div>
      <div class="input-div">
        <input id="password" type="text" placeholder="Password" class="input">
        <hr class="line">
      </div>
      <button class="button bg-green-500 mt-12" @click="submit">
        Log In
      </button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    submit(event) {
      let email = document.getElementById("email");
      let password = document.getElementById("password");
      const users = $http.$get('http://localhost:3000/customers');
      console.log(users);
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
