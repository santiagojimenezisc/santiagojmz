<template>
  <div id="footer">
    <footer class="container">
      <div class="row">
        <div class="col-lg-4 col-md-4 col-sm-6">
          <div class="logo-footer">
            <h2>Santi</h2>
            <h4>Desarrollador Frontend</h4>
          </div>
        </div>
        <div class="col-lg-4 col-md-4 col-sm-6 text-center footer-nav">
          <a href="">Sobre mí</a>
          <a href="">Portafolio</a>
          <a href="">Contacto</a>
        </div>
        <div class="col-lg-4 col-md-4 col-sm-12 text-center footer-redes">
          <a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
          <a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
          <a href=""><font-awesome-icon :icon="['fab', 'dribbble']" /></a>
        </div>
      </div>
      <div class="row">
        <div class="made-by">
          <h6>Hecha con pasión by Santi.</h6>
        </div>
      </div>
    </footer>
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style scoped>
.made-by{
    display: flex;
    justify-content: center;
    margin: 75px 0px 0px 0px;
}
.col-sm-12 {
  margin: 5px 0px;
}
.footer-redes {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: 25px;
}
.footer-redes a {
  font-size: 24px !important;
}
.footer-nav {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

#footer {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow-x: hidden;
  width: 100%;
  overflow-y: hidden;
  background-color: #0085ff;
  color: #fff;
  position: absolute;
  bottom: 0;
  left: 0;
  padding: 75px 0px 25px 0px;
}
.logo-footer {
  text-align: left;
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
@media only screen and (max-width: 768px) {

  .footer-nav {
    flex-direction: column;
    align-items: flex-end;
  }

.footer-redes {
  justify-content: start;

}
}

h2 {
  font-weight: 700;
  font-size: 36px;
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