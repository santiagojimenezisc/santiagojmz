<template>
  <div id="Header">
    <header class="container">
      <div class="brand">
        <a href="#">Santi</a>
      </div>
      <nav class="nav">
        <ul class="navbar__links">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre mí</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Portafolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contacto</a>
          </li>
        </ul>
      </nav>
      <nav class="nav-movile">
        <font-awesome-icon :icon="['fas', 'bars']" size="lg" :style="{ color: '#0085ff' }"/>
      </nav>
    </header>
  </div>
</template>
<script>
export default {
  name: "Header",
};
</script>
<style scoped>
.nav-movile{
  display: none;
}
header {
  background-color: #fcfdff;
  width: 100%;
  overflow-x: hidden;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px 0px;
}
.brand a{
text-decoration: none;
color:#020F1B;
font-weight: 700;
  font-size: 34px;
}
nav{
  order:2;
}
.navbar__links {
  list-style: none;
}
.navbar__links li {
  display: inline-block;
  padding: 0px 10px;
}
.navbar__links a{
  text-decoration: none;
  font-size: 16px;
  color: #020F1B;
  font-weight: 500;
  transition: all 0.3s ease-in-out 0s;
}
.navbar__links a:hover{
   color:#0085ff;
   transition: all 0.3s ease-in-out 0s;
}
.navbar__links .active{

 color:#0085ff;
}
/*
* Santiago Jimenez 02/10/21
* Móvil responsivo pantallas menores a 768px  
*/
@media only screen and (max-width: 768px) {
  #Header{
    border-bottom: black;
  }
  .nav{
    display: none;
  }
  .nav-movile{
    display: flex;
  }
}

</style>