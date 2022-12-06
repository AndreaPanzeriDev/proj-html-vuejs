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
    <presentation :arrayTwitter="arrayTwitter"/>
    <sponsor :arraySponsor="arraySponsor"/>
    <footerComp :arrayGallery="arrayGallery"/>
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
import presentation from './presentationComp.vue'
import sponsor from './sponsorComp.vue'
import footerComp from './footerComp.vue'

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
        ticket,
        presentation,
        sponsor,
        footerComp
    },
    props:{
      arrayAboutUs: Array,
      arraySpeakers: Array,
      arrayPrograms: Array,
      arrayRecentNews: Array,
      arrayTicket: Array,
      arrayTwitter: Array,
      arraySponsor: Array,
      arrayGallery: Array
    },
}
</script>

<style>

</style>