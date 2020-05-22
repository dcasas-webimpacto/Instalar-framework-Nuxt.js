<template>
  <div
    class="col-11 form-group inner-addon right-addon fila9-1"
    id="show_hide_password"
  >
    <label for="exampleInputPassword1" id="passregistro">Contraseña</label>
    <input type="password" class="form-control" id="casillapass" />
    <a class="icone" id="enlacee" @click="mostrarpass"
      ><img id="imagenpass" src="../assets/hide.svg"
    /></a>
  </div>
</template>

<script>
export default {
  methods: {
    mostrarpass() {
      var campo = document.getElementById("casillapass");
      var imagenojo = document.getElementById("imagenpass");
      if (campo.type == "password") {
        campo.type = "text";
        imagenojo.setAttribute("src", "/_nuxt/assets/show.svg");
      } else if (campo.type == "text") {
        campo.type = "password";
        imagenojo.setAttribute("src", "/_nuxt/assets/hide.svg");
        // imagenojo.attr("src", "../assets/hide.svg");
      }
    }
  }
};
</script>
<style scoped>
@media (max-width: 766px) {
  .icone img {
    width: 25px;
    height: 25px;
  }
  .inner-addon {
    position: relative;
  }
  .inner-addon .icone {
    position: absolute;
    padding: 0%;
    /* pointer-events: none; */
  }
  .right-addon .icone {
    background-size: contain;
    border: none;
    outline: none;
    margin-top: 0px;

    z-index: 2;
    opacity: 0.3;
    right: 30px;
    top: 33px;
  }
  .right-addon input {
    padding-right: 30px;
  }
  .fila9-1 {
    margin-left: 20px;
  }
  #passregistro {
    margin-bottom: 6px;
    font-family: Lato-Regular;
    font-size: 13px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 13px;
  }
  #casillapass {
    height: 45px;
    width: 99%;
  }
}
@media (min-width: 766px) {
  .icone img {
    width: 25px;
    height: 25px;
  }
  .inner-addon {
    position: relative;
  }
  .inner-addon .icone {
    position: absolute;
    padding: 0%;
    /* pointer-events: none; */
  }
  .right-addon .icone {
    background-size: contain;
    border: none;
    outline: none;
    margin-top: 0px;

    z-index: 2;
    opacity: 0.3;
    right: 57px;
    top: 33px;
  }
  .right-addon input {
    padding-right: 30px;
  }
  .fila9-1 {
    margin-left: 35px;
  }
  #passregistro {
    margin-bottom: 6px;
    font-family: Lato-Regular;
    font-size: 13px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 13px;
  }
  #casillapass {
    height: 45px;
    width: 90%;
  }
}
</style>
