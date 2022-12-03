<template>
  <div id="header">
    <img src="../assets/img/logo.png" alt="logo" />
    <div class="sectionLink">
      <li class="dropdonMenu"><a href="#">HOME</a></li>
      <li class="dropdonMenu"><a href="#">PAGES</a></li>
      <li class="dropdonMenu"><a href="#">PROGRAMS</a></li>
      <li class="dropdonMenu"><a href="#">TICKETS</a></li>
      <li class="dropdonMenu"><a href="#">SPEAKERS</a></li>
      <li class="dropdonMenu"><a href="#">PAPERS</a></li>
      <li class="dropdonMenu"><a href="#">BLOG</a></li>
      <li class="dropdonMenu"><a href="#">SHORTCODES</a></li>
      <li class="dropdonMenu"><a href="#">|</a></li>
      <li class="dropdonMenu">
        <a href="#"><i class="fa-solid fa-magnifying-glass"></i></a>
        <ul>
            <li class="dropdownSelection">cvvrvrvrrr</li>
            <li class="dropdownSelection">c</li>
            <li class="dropdownSelection">c</li>
            <li class="dropdownSelection">c</li>
            <li class="dropdownSelection">c</li>
        </ul>
      </li>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
/*******************
       HEADER
*******************/
#header {
  padding: 25px;
  width: 70%;
  margin: auto;
  display: flex;
  justify-content: space-between;
}

/*******************
     DROPDOWN
*******************/

.dropdonMenu {
  list-style: none;
  margin: 0 10px;
  position: relative;
}

.dropdonMenu > ul{
    display: none;
}

.dropdonMenu:hover > ul{
    display: block;
    position: absolute;
    right: 0;
    top: 0;
    width: 25px;
}

.dropdownSelection{
    list-style: none;
    background-color: black;
    opacity: 0.6;
    width: 160px;
    color: white;
    padding: 10px;
}


/*******************
         A
*******************/

a {
  text-decoration: none;
  color: #8e8e8e;
  font-size: 13px;
  font-weight: 900;
}

a:hover {
  padding-bottom: 3px;
  border-bottom: 3px solid salmon;
}



/*******************
    SECTIONLINK
*******************/

.sectionLink {
  display: flex;
}
</style>