<template>
  <div>
    <EventComp/>
    <QuestionComp :arrayAboutUs="arrayAboutUs"/>
    <SubscribeComp/>
    <speakerComp :arraySpeakers="arraySpeakers"/>
    <programCard :arrayPrograms="arrayPrograms"/>
    <googleMaps/>
    <LocationComp/>
    <recentNews :arrayRecentNews="arrayRecentNews"/>
    <ticket :arrayTicket="arrayTicket"/>

  </div>
</template>

<script>
import EventComp from './EventComp.vue'
import QuestionComp from './QuestionComp.vue'
import SubscribeComp from './SubscribeComp.vue'
import speakerComp from './speaker/speakerComp.vue'
import programCard from './program/programCard.vue'
import googleMaps from './GoogleMapsComp.vue'
import LocationComp from './LocationComp.vue'
import recentNews from './recentNews.vue'
import ticket from './ticketComp.vue'

export default {
    components:{
        EventComp,
        QuestionComp,
        SubscribeComp,
        speakerComp,
        programCard,
        googleMaps,
        LocationComp,
        recentNews,
        ticket

    },
    props:{
      arrayAboutUs: Array,
      arraySpeakers: Array,
      arrayPrograms: Array,
      arrayRecentNews: Array,
      arrayTicket: Array
    },
}
</script>

<style>

</style>