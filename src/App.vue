<template>
  <div id="app">
    <HeaderComp/>
    <MainComp :arrayAboutUs="aboutUs" :arraySpeakers="speakers" :arrayPrograms="programs" :arrayRecentNews="recentNews" :arrayTicket="ticket" :arrayTwitter="twitter" :arraySponsor="sponsor" :arrayGallery="gallery"/>
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
        {date: '23 May 2023', time: '09:00 - 10:30', name:'PATRICK SPENCER', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r eorinoienfoienrfne noerfneornno fen noerfno ien ornfeon onernfo erinfoien noin rfnioenrfonernfoen irn foner in ofenronf oenrfonefoiern eonir oeon oe f voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-1-150x150.jpg'},
        {date: '24 May 2023', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-2-150x150.jpg'},
        {date: '25 May 2023', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-3-150x150.jpg'},
        {date: '26 May 2023', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-4-150x150.jpg'},
        {date: '27 May 2023', time: '09:00 - 10:30', name:'MARGARET SMITH', title: 'WELCOMING AND INTRODUCTION', description: 'orein voinvre veonvoernvovnoe vn r vernvoienve voenrvnreonveonv nibr vrei veirbviubibs cewiiubbf', picture: 'speaker-5-150x150.jpg'},
      ],
      recentNews:[
        {img: 'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg', date: '03 Dec 2013', comments: '0', title: 'SEDIAL EIUSMOD TEMPOR', phrase: 'Lorem ipsum dolor sit amet, consectetur adipisici elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Idque Caesaris facere voluntate liceret: sese habere.... '},
        {img: 'photodune-8797753-multiethnic-people-with-startup-business-t (2).jpg', date: '03 Dec 2013', comments: '2', title: 'DONEC LUCTUS IMPERDIET', phrase: 'Lorem ipsum dolor sit amet, consectetur adipisici elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Idque Caesaris facere voluntate liceret: sese habere.... '},
        {img: 'photodune-8522811-speaker-at-business-conference-and-present (2).jpg', date: '03 Dec 2013', comments: '5', title: 'MAGNA PARS STUDIORUM', phrase: 'Lorem ipsum dolor sit amet, consectetur adipisici elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Idque Caesaris facere voluntate liceret: sese habere.... '},
      ],
      ticket: [
        {name: 'ONE DAY PASS', price: 'FREE', bonus: [
          'One Day Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '50USD Voucher For Next Event'
        ]},
        {name: 'FOUR DAYS PASS', price: '750.00 USD', bonus: [
          'Four Days Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '100USD Voucher For Next Event'
        ]},
        {name: 'TWO DAYS PASS', price: '550.00 USD', bonus: [
          'Two Days Access',
          'Coffee Break',
          'Lunch(International buffet)',
          'Document Sheets',
          '70USD Voucher For Next Event'
        ]}
      ],
      twitter: [
        "Next I'm buying Coca-Cola to put the cocaine back in",
        "No one is born hating another person because of the color of his skin or his background or his religion...",
        "Kobe was a legend on the court and just getting started in what would have been just as meaningful a second act. To lose Gianna is even more heartbreaking to us as parents. Michelle and I send love and prayers to Vanessa and the entire Bryant family on an unthinkable day."

      ],
      sponsor:[
        'banner-1.jpg',
        'banner-2.jpg',
        'banner-3.jpg',
        'banner-4.jpg',
        'banner-5.jpg',
        'banner-6.jpg'
      ],

      gallery:[
        'photodune-6745585-modern-creative-workspace-m-150x150.jpg',
        'card01-150x150.jpg',
        '13349065283_64d09b067c_o-150x150.jpg',
        'card04-150x150.jpg',
        'photodune-6745606-man-wristwatch-calendar-key-and-glasses-on.jpg',
        'photodune-8522811-speaker-at-business-conference-and-present (1).jpg',
        'photodune-8523683-speaker-at-business-convention-and-present.jpg',
        'photodune-8795110-overhead-of-essentials-denim-clothes-m-150.jpg',
        'photodune-8797753-multiethnic-people-with-startup-business-t (1).jpg',
        'speaker-1-150x150.jpg',
        'photodune-6745585-modern-creative-workspace-m-150x150.jpg',
        'speaker-3-150x150.jpg',
      ]
      
    }
  }
}
</script>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

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

.pb-50{
  padding-bottom: 50px;
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

.o-9{
  opacity: 0.9;
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

.pt-15{
  padding-top: 15px;
}

.w-20{
  width: 20%;
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

.bblack{
  background-color: black;
}
</style>
