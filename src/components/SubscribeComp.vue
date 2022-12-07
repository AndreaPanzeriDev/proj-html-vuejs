<template>
  <div id="subscribe">
    <div class="container m-auto">
      <div class="d-flex blocks">
        <div class="block">
          <h1>326</h1>
          <h6>giorni</h6>
        </div>
        <div class="block">
          <h1>326</h1>
          <h6>giorni</h6>
        </div>
        <div class="block">
          <h1>326</h1>
          <h6>giorni</h6>
        </div>
        <div class="block">
          <h1>326</h1>
          <h6>giorni</h6>
        </div>
      </div>
      <h1>SUBSCRIBE FOR MORE UPDATE</h1>
      <div class="d-flex space-around">
        <input type="email" v-model="mail" placeholder="Please file your email">
        <button v-on:click="checkemail()" class="button text-white">SUBSCRIBE</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubscribeComp",
  data(){
    return{
      mail: ''
    }
  },
  methods:{
    checkemail(){
      if(this.mail == ''){
        alert("the label is empty")
      }if(!this.mail.includes("@")){
        alert('you forgot the @')
      }else{
        alert('check your mailbox')
      }
    }
  }
};
</script>

<style scoped>
#subscribe {
  background-image: url("../assets/img/coutdown-bg1.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  margin-top: 50px;
  height: 500px;
  display: flex;
}

.blocks{
  justify-content: space-around;
}
.block {
  background-color: black;
  opacity: 0.7;
  padding: 2px 10px;
  border-radius: 5px;
  margin: auto 5px;
  color: white;
}

.d-flex > input{
  width: 300px;
  border-radius: 10px;
  border: none;
}
</style>