<template>
  <div>
    <Card/>
  </div>
</template>

<script>
import Card from './card/ticketCard.vue'


export default {
    name: 'ticketComp',
    components:{
        Card
    },
    props:{
      arrayTicket: Array
    }
}
</script>

<style>

</style>