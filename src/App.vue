<template>
  <div id="app">
    <HeaderComp/>
    <MainComp :arrayAboutUs="aboutUs" :arraySpeakers="speakers" :arrayPrograms="programs" :arrayRecentNews="recentNews" :arrayTicket="ticket" :arrayTwitter="twitter" :arraySponsor="sponsor"/>
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
        {date: '23 May 2016', time: '09:00 - 10:30', name:'PATRICK SPENCER', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r eorinoienfoienrfne noerfneornno fen noerfno ien ornfeon onernfo erinfoien noin rfnioenrfonernfoen irn foner in ofenronf oenrfonefoiern eonir oeon oe f voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-2-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-3-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-4-150x150.jpg'},
        {date: '23 May 2016', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-5-150x150.jpg'},
      ],
      recentNews:[
        {img: 'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg', date: '03 Dec 2013', comments: '0', title: 'SEDIAL EIUSMOD TEMPOR', phrase: 'loreeoimfoern rionenfier reinfeirunfe fe irbfnienfienrf efiuenrfiuenfrunef eiunfeiunrfienr feiunrfienfie'},
        {img: 'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg', date: '03 Dec 2013', comments: '0', title: 'SEDIAL EIUSMOD TEMPOR', phrase: 'loreeoimfoern rionenfier reinfeirunfe fe irbfnienfienrf efiuenrfiuenfrunef eiunfeiunrfienr feiunrfienfie'},
        {img: 'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg', date: '03 Dec 2013', comments: '0', title: 'SEDIAL EIUSMOD TEMPOR', phrase: 'loreeoimfoern rionenfier reinfeirunfe fe irbfnienfienrf efiuenrfiuenfrunef eiunfeiunrfienr feiunrfienfie'},
      ],
      ticket: [
        {name: 'ONE DAY PASS', price: 'FREE', bonus: [
          'One Day Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '50USD Voucher For Next Event'
        ]},
        {name: 'ONE DAY PASS', price: 'FREE', bonus: [
          'One Day Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '50USD Voucher For Next Event'
        ]},
        {name: 'ONE DAY PASS', price: 'FREE', bonus: [
          'One Day Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '50USD Voucher For Next Event'
        ]}
      ],
      twitter: [
        "Next I'm buying Coca-Cola to put the cocaine back in",
        "No one is born hating another person because of the color of his skin or his background or his religion...",
        "Kobe was a legend on the court and just getting started in what would have been just as meaningful a second act. To lose Gianna is even more heartbreaking to us as parents. Michelle and I send love and prayers to Vanessa and the entire Bryant family on an unthinkable day."

      ],
      sponsor:[
        'banner-1',
        'banner-2',
        'banner-3',
        'banner-4',
        'banner-5',
        'banner-6'
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

.mr-30{
  margin-right: 30px;
}

.my-15{
  margin: 15px 0;
}

.my-30{
  margin: 30px 0;
}

.py-15{
  padding: 15px 0;
}

.py-25{
  padding: 25px 0;
}

.pt-25{
  padding-top: 25px;
}

.o-5{
  opacity: 0.5;
}

.o-7{
  opacity: 0.7;
}

.fs-1{
  font-size: 1.5rem;
}

.fs-2{
  font-size: 2rem;
}

.fs-3{
  font-size: 3rem;
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

.w-100{
  width: 100%;
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

.bscarlet{
  background-color: #f7260c;
}

.bsand{
  background-color: #f3f3f3;
}

.sand{
  color: #f3f3f3
}

.bwhite{
  background-color: white;
}

.lightblue{
  color: rgb(43, 185, 232);
}
</style>
