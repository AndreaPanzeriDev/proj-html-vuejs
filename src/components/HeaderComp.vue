<template>
  <div id="header">
    <img src="../assets/img/logo.png" alt="logo" />
    <div class="sectionLink">
      <li class="dropdonMenu">
        <a href="#">HOME</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Home 1</a></li>
          <li class="dropdownSelection"><a href="#">Home 2</a></li>
        </ul>
      </li>
      <li class="dropdonMenu">
        <a href="#">PAGES</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Page1</a></li>
          <li class="dropdownSelection"><a href="#">Page2</a></li>
          <li class="dropdownSelection"><a href="#">Page3</a></li>
          <li class="dropdownSelection"><a href="#">Page4</a></li>
          <li class="dropdownSelection"><a href="#">Page5</a></li>
        </ul>
      </li>
      <li class="dropdonMenu">
        <a href="#">PROGRAMS</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Program1</a></li>
          <li class="dropdownSelection"><a href="#">Program2</a></li>
          <li class="dropdownSelection"><a href="#">Program3</a></li>
        </ul>
      </li>
      <li class="dropdonMenu">
        <a href="#">TICKETS</a>
      </li>
      <li class="dropdonMenu">
        <a href="#">SPEAKERS</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Speakear1</a></li>
          <li class="dropdownSelection"><a href="#">Speaker2</a></li>
          <li class="dropdownSelection"><a href="#">Speaker3</a></li>
          <li class="dropdownSelection"><a href="#">Speaker4</a></li>
        </ul>
      </li>
      <li class="dropdonMenu">
        <a href="#">PAPERS</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Paper1</a></li>
          <li class="dropdownSelection"><a href="#">Papaer2</a></li>
        </ul>
      </li>
      <li class="dropdonMenu">
        <a href="#">BLOG</a>
      </li>
      <li class="dropdonMenu">
        <a href="#">SHORTCODES</a>
        <ul>
          <li class="dropdownSelection"><a href="#">Examlpe1</a></li>
          <li class="dropdownSelection"><a href="#">Example2</a></li>
          <li class="dropdownSelection"><a href="#">Example3</a></li>
          <li class="dropdownSelection"><a href="#">Example4</a></li>
        </ul>
      </li>
      <li class="dropdonMenu"><a href="#">|</a></li>
      <li class="dropdonMenu">
        <a href="#"><i class="fa-solid fa-magnifying-glass"></i></a>
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
  height: 70px;
  width: 70%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#header > img{
  height: fit-content;
}
/*******************
     DROPDOWN
*******************/

.dropdonMenu {
  list-style: none;
  margin: 0 10px;
  position: relative;
  height: 100%;
  display: flex;
  align-items: center;
}

.dropdonMenu > ul {
  display: none;
}

.dropdonMenu:hover > ul {
  display: block;
  position: absolute;
  right: 15px;
  top: 50px;
  width: 25px;
  transition-delay: 1s;
}

.dropdownSelection {
  list-style: none;
  background-color: black;
  opacity: 0.6;
  width: 160px;
  color: white;
  padding: 10px;
}

.dropdownSelection:hover{
  display: block;
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
  height: 100%;
}
</style>