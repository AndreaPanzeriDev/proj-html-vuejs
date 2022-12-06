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

export default {
    components:{
        EventComp,
        QuestionComp,
        SubscribeComp,
        speakerComp,
        programCard,
        googleMaps,
        LocationComp,
        recentNews

    },
    props:{
      arrayAboutUs: Array,
      arraySpeakers: Array,
      arrayPrograms: Array,
      arrayRecentNews: Array
    },
}
</script>

<style>

</style>