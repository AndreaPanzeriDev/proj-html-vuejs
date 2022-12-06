<template>
  <div>
    <EventComp/>
    <QuestionComp :arrayAboutUs="arrayAboutUs"/>
    <SubscribeComp/>
    <speakerComp :arraySpeakers="arraySpeakers"/>
    <programCard :arrayPrograms="arrayPrograms"/>
    <googleMaps/>
  </div>
</template>

<script>
import EventComp from './EventComp.vue'
import QuestionComp from './QuestionComp.vue'
import SubscribeComp from './SubscribeComp.vue'
import speakerComp from './speaker/speakerComp.vue'
import programCard from './program/programCard.vue'
import googleMaps from './GoogleMapsComp.vue'

export default {
    components:{
        EventComp,
        QuestionComp,
        SubscribeComp,
        speakerComp,
        programCard,
        googleMaps

    },
    props:{
      arrayAboutUs: Array,
      arraySpeakers: Array,
      arrayPrograms: Array
    },
}
</script>

<style>

</style>