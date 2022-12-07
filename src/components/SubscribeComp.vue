<template>
  <div id="subscribe">
    <div class="container m-auto">
      <div class="d-flex blocks">
        <div class="block">
          <h1>{{displaydays}}</h1>
          <h6>DAYS</h6>
        </div>
        <div class="block">
          <h1>{{displayhours}}</h1>
          <h6>HOURS</h6>
        </div>
        <div class="block">
          <h1>{{displayminutes}}</h1>
          <h6>MINUTES</h6>
        </div>
        <div class="block">
          <h1>{{displayseconds}}</h1>
          <h6>SECONDS</h6>
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
      mail: '',
      displaydays: 0,
      displayhours: 0,
      displayminutes: 0,
      displayseconds: 0,
    }
  },
  computed:{
    _seconds: () => 1000,
    _minutes(){
      return this._seconds * 60
    },
    _hours(){
      return this._minutes * 60
    },
    _days(){
      return this._hours * 24
    }
  },
  mounted(){
    this.remainingTime()
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
    },

    remainingTime(){
      const timer = setInterval(() => {
        const now  = new Date();
        const end = new Date(2023, 4, 23, 10, 10, 10, 10);
        const distance = end.getTime() - now.getTime()

        if(distance < 0){
          clearInterval(timer);
          return
        }

        const days = Math.floor((distance / this._days));
        const hours = Math.floor((distance % this._days) / this._hours);
        const minutes = Math.floor((distance % this._hours) / this._minutes);
        const seconds = Math.floor((distance % this._minutes) / this._seconds);

        this.displayseconds = seconds < 10 ? "0" + seconds : seconds;
        this.displayminutes = minutes < 10 ? "0" + minutes : minutes;
        this.displayhours = hours < 10 ? "0" + hours : hours;
        this.displaydays = days < 10 ? "0" + days : days;
      }, 1000 );
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