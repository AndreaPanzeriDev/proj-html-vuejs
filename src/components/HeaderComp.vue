<template>
  <div id="header">
    <img src="../assets/img/logo.png" alt="logo">
    <div class="sectionLink">
        <li><a href="#">HOME</a></li>
        <li><a href="#">PAGES</a></li>
        <li><a href="#">PROGRAMS</a></li>
        <li><a href="#">TICKETS</a></li>
        <li><a href="#">SPEAKERS</a></li>
        <li><a href="#">PAPERS</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">SHORTCODES</a></li>
        <li><a href="#">|</a></li>
        <li><a href="#"><i class="fa-solid fa-magnifying-glass"></i></a></li>
        
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

/*******************
       HEADER
*******************/
#header{
    padding: 25px;
    width: 60%;
    margin: auto;
    display: flex;
    justify-content: space-between;
}

/*******************
        LI
*******************/

li{
    list-style: none;
}

/*******************
         A
*******************/

a{
    text-decoration: none;
    color: #8e8e8e;
    font-size: 13px;
    font-weight: 900;
    margin: 0 10px;
}

/*******************
    SECTIONLINK
*******************/

.sectionLink{
    display: flex;
}


</style>