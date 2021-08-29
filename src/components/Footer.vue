<template>
  <div id="footer" class="">
    <footer class="container">
      <div class="row">
        <div class="col-lg-4 col-md-4 col-sm-12">
          <div class="logo-footer">
            <h2>Santi</h2>
            <h4>Desarrollador Frontend</h4>
          </div>
        </div>
        <div class="col-lg-4 col-md-4 col-sm-12 text-center">Navegación</div>
        <div class="col-lg-4 col-md-4 col-sm-12 text-center">Redes sociales</div>
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
#footer {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow-x: hidden;
  width: 100%;
  overflow-y: hidden;
  background-color: #0085ff;
  max-height: 200px;
  color: #fff;
  position: absolute;
  bottom: 0;
  left: 0;
  padding: 50px 0;
}
.logo-footer {
  text-align: left;
}
@media only screen and (max-width: 768px) {
  .logo-footer {
  text-align: center;
}
}

h4 {
  font-size: 16px;
  font-weight: 500;
  color:#C3E2FF;
}
</style>