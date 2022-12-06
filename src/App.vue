<template>
  <div id="app">
    <HeaderComp/>
    <MainComp :arrayAboutUs="aboutUs" :arraySpeakers="speakers" :arrayPrograms="programs"/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
  },
  data(){
    return{
      aboutUs: [
        {icon: 'fa-solid fa-trophy', title: 'WHO WE ARE', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
        {icon: 'fa-solid fa-bolt', title: 'WHAT WE DO', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
        {icon: 'fa-solid fa-question', title: 'WHY US', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
      ],
      speakers: [
        {person: 'speaker-1.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-2.jpg', name: 'JANET JONES', job: "NewYork Post't GM"},
        {person: 'speaker-3.jpg', name: 'ANGELINA HOLY', job: "Starbuck's CEO"},
        {person: 'speaker-4.jpg', name: 'MICHEAL DOVER', job: "Maxii's Manager"},
        {person: 'speaker-5.jpg', name: 'ANGELINA HOLY', job: 'S&P Analyzer'},
        {person: 'speaker-6.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-7.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-8.jpg', name: 'MARGARET SMITH', job: 'S&P Analyzer'},
      ],
      programs: [
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r eorinoienfoienrfne noerfneornno fen noerfno ien ornfeon onernfo erinfoien noin rfnioenrfonernfoen irn foner in ofenronf oenrfonefoiern eonir oeon oe f voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
      ]
      
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}



.d-flex {
  display: flex;
}

.text-center{
  text-align: center;
}

.justify-content-center{
  justify-content: center;
}

.text-white{
  color: white;
}

.fw-bold{
  font-weight: bold;
}

.ms-5{
  margin: 0 5px;
}
.mt-20{
  margin-top: 20px;
}

.mt-50{
  margin-top: 50px;
}

.my-20{
  margin: 20px 0;
}

.mr-10{
  margin-right: 10px;
}

.pt-25{
  padding-top: 25px;
}

.o-7{
  opacity: 0.7;
}

.fs-2{
  font-size: 2rem;
}

.align-self-center{
  align-self: center;
}

.align-items-center{
  align-items: center;
}

.text-black{
  color: black;
}

.button{
  padding: 10px 15px;
  border: none;
  border-radius: 5px;
  background-color: #f7260c;
}

.m-auto{
  margin: auto;
}

.space-around{
  justify-content: space-around;
}

.space-between{
  justify-content: space-between;
}


.italic{
  font-style: italic;
}

a{
  text-decoration: none;
}

.w-25{
  width: 25%;
}

.w-50{
  width: 50%;
}

.w-75{
  width: 75%;
}
/***********************
        COLORS
************************/

.cloud{
  color: #c6c1bd;
}

.dustyGray{
  color: #9c9c9c;
}

.scarlet{
  color: #f7260c;
}

.bsand{
  color: #f3f3f3;
}
</style>
