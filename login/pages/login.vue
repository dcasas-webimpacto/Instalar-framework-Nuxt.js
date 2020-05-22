<template>
  <div class="container">
    <div class="row fila20 justify-content-center">
      <div class="contenedorPrincipal ">
        <div class="contenedorImagen">
          <div class="row fila1">
            <div class="col-5 col-xs-5 col-sm-5 pl-2 pl-sm-3 c1">
              <img id="img1" src="../assets/go-back.svg" />
              <span class="span1">
                Volver
              </span>
            </div>
            <div class="col-7 col-xs-7 col-sm-7 pr-2 c">
              <span class="span2">
                Nueva cuenta
              </span>
              <img id="img2" src="../assets/User-plus.svg" />
            </div>
          </div>
          <div class="row fila2">
            <img
              src="../assets/Nutritienda-simple_logo.svg"
              id="logogrande"
              alt=""
            />
          </div>
          <div class="row fila3">
            <p id="login">Login</p>
          </div>
        </div>
        <div class="row fila4">
          <p id="accede">¡Accede a tu cuenta para disfrutar de tus ventajas!</p>
        </div>
        <div class="row fila5">
          <hr class="hr" />
          <p class="letrasacceso">ACCESO RÁPIDO CON REDES SOCIALES</p>
          <hr class="hr" />
        </div>
        <div class="row fila6">
          <div class="col-2 fila6-1">
            <img
              class="iconosredes"
              id="face"
              src="../assets/connect-Facebook-42px.svg"
              alt=""
            />
          </div>
          <div class="col-2 fila6-2">
            <img
              class="iconosredes"
              id="google"
              src="../assets/connect-Google-42px.svg"
              alt=""
            />
          </div>
          <div class="col-2 fila6-3">
            <img
              class="iconosredes"
              id="twitter"
              src="../assets/connect-Twitter-42px.svg"
              alt=""
            />
          </div>
        </div>
        <div class="row fila7">
          <hr class="hr2" />
          <p class="letrasacceso">ACCESO CON EMAIL Y CONTRASEÑA</p>
          <hr class="hr2" />
        </div>
        <form>
          <div class="row fila8">
            <div class="col-11 form-group fila8-1">
              <label for="exampleInputEmail1" id="emailregistro">Email</label>
              <input type="email" class="form-control" id="casillaemail" />
            </div>
          </div>
          <div class="row fila9">
            <iconopass />
            <!--COMPONENTE ICONO PASSWORD -->
          </div>
          <div class="row justify-content-center fila10">
            <div class="col-4 col-md-4 col-lg-4 fila10-1">
              <pruebacheck />
              <!--COMPONENTE CHECKBOX -->
            </div>
            <div class="col-7 col-md-5 col-lg-5 fila10-2">
              <a href="" id="letrascontra">¿Has olvidado tu contraseña?</a>
            </div>
          </div>
          <div class="row fila11">
            <div class="col-12 fila11-1">
              <boton />

              <!--COMPONENTE BOTON -->
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import boton from "@/components/boton";
import iconopass from "@/components/iconopass";
import pruebacheck from "@/components/pruebacheck";
// import pruebacomponente from "@/components/pruebacomponente";
export default {
  components: {
    boton,
    iconopass,
    pruebacheck
    // pruebacomponente
  }
};
</script>

<style src="~/assets/css/main.css" >
