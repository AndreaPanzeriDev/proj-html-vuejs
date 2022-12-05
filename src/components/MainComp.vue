<template>
  <div>
    <EventComp/>
    <QuestionComp :arrayAboutUs="arrayAboutUs"/>
  </div>
</template>

<script>
import EventComp from './EventComp.vue'
import QuestionComp from './QuestionComp.vue'

export default {
    components:{
        EventComp,
        QuestionComp
    },
    props:{
      arrayAboutUs: Array
    },
}
</script>

<style>

</style>