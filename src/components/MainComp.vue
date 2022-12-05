<template>
  <div>
    <EventComp/>
    <QuestionComp :arrayAboutUs="arrayAboutUs"/>
    <SubscribeComp/>
  </div>
</template>

<script>
import EventComp from './EventComp.vue'
import QuestionComp from './QuestionComp.vue'
import SubscribeComp from './SubscribeComp.vue'

export default {
    components:{
        EventComp,
        QuestionComp,
        SubscribeComp
    },
    props:{
      arrayAboutUs: Array
    },
}
</script>

<style>

</style>