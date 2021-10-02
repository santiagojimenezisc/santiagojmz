<template >
  <footer id="Footer">
    <div class="container">
    <section class="footer-content">
      <div class="">
        <div class="logo-footer">
          <h2>Santi</h2>
          <h4>Desarrollador Frontend</h4>
        </div>
      </div>
      <div class="footer-nav">
        <a href="">Inicio</a>
        <a href="">Sobre mí</a>
        <a href="">Portafolio</a>
        <a href="">Contacto</a>
        
      </div>
      <div class="footer-redes">
        <a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
        <a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
        <a href=""><font-awesome-icon :icon="['fab', 'dribbble']" /></a>
      </div>
    </section>
    <section class="footer-made-by">
      <h6>Hecha con ❤ por Santi.</h6>
    </section>
    </div>

  </footer>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style scoped>
#Footer {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  overflow-x: hidden;
  overflow-y: hidden;
  background-color: #0085ff;
  color: #fff;
  position: absolute;
  width: 100vw;
  bottom: 0;
  left: 0;
  padding: 25px 0px 25px 0px;
}
.logo-footer {
 display: flex;
 flex-direction: column;
}
.footer-redes {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: 25px;
}
.footer-made-by {
  display: flex;
  justify-content: center;
  margin: 50px 0px 0px 0px;
}
.footer-redes a {
  font-size: 24px !important;
}
.footer-nav {
  display: flex;
  flex-direction: row;
  gap:10px;
  justify-content: space-between;
}
.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

a {
  color: #fff;
  text-decoration: none;
  transition: 0.4s;
}
a:hover {
  color: #00386b;
  transition: 0.4s;
}
@media only screen and (max-width: 767px) {
  .footer-content{
    flex-direction: column;
    gap:25px 25px;
  }
  .footer-nav {
    order:3;
    flex-direction: column;
    align-items: center;
  }
  .logo-footer{
    order: 1;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .footer-redes {
    order:2;
    justify-content: start;
  }
}
@media (max-width: 1024px ) and (min-width: 768px)  {
  .footer-content{
    flex-direction: row;
  }
  .logo-footer{
    flex-direction:column;
    justify-content: start;
  }
  .footer-nav {
}
}

h2 {
  font-weight: 700;
  font-size: 32px;
}
h4 {
  font-size: 16px;
  font-weight: 300;
  color: #c3e2ff;
}
#footer h6 {
  font-size: 14px;
  color: #87c5ff;
  text-align: center;
  font-weight: 400;
}
</style>