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
            <div class="col-5 col-md-4 col-lg-4 fila10-1">
              <label class="custom-radio-checkbox">
                <input class="custom-radio-checkbox__input" type="checkbox" />
                <span
                  class="custom-radio-checkbox__show custom-radio-checkbox__show--checkbox"
                ></span>
                Recuérdame
              </label>
            </div>
            <div class="col-6 col-md-5 col-lg-5 fila10-2">
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
// import pruebacomponente from "@/components/pruebacomponente";
export default {
  components: {
    boton,
    iconopass
    // pruebacomponente
  },
  methods: {
    clickMe() {
      alert("hola mundo");
    }
  }
};
</script>
<style>
@font-face {
  font-family: "Nexa-Xbold";
  src: url("/login/static/Nexa/Nexa_V2_2020/WEB/NexaTextDemo-Bold.woff")
    format("woff");
}
@font-face {
  font-family: "Nexa-Bold";
  src: url("/login/static/Nexa/Nexa_V2_2020/WEB/NexaDemo-Bold.woff")
    format("woff");
}
@font-face {
  font-family: "Lato-Regular";
  /* src: url("static/Lato-Regular/Lato-Regular.ttf"); */
  src: url("/login/static/Lato-Regular/Lato-Regular.ttf") format("truetype");
}

body {
  background-image: linear-gradient(#fa2398 100%, #dd1f94 100%);
}
@media (max-width: 766px) {
  body {
    background-image: none;
  }
}
.custom-radio-checkbox span {
  font-family: Lato-Regular;
  font-size: 14px;
  color: #3b3b3b;
  letter-spacing: 0;
  line-height: 20px;
}
.custom-radio-checkbox__input {
  margin-left: 15px;
}
/* input[type="checkbox"] {
  display: none;
  border: 1px;
}

input[type="checkbox"] + label {
  height: 50px;
  width: 50px;
  background-image: none;
  display: inline-block;
}

input[type="checkbox"]:checked + label {
  background-image: url("../assets/check_for_checkbox.svg");
} */

.checkbox {
  width: 22px;
  height: 18px;
  border: 1px solid #c0c2c8;
  border-radius: 10%;
}
.checked {
  background: url("../assets/check_for_checkbox.svg") no-repeat 30% 60%;
  border: solid black 2px;
}
#show_hide_password {
  z-index: 1;
}

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

  .contenedorPrincipal {
    width: 100%;
    height: 660px;
    background-color: white;
    position: relative;
  }
  .contenedorImagen {
    background-image: url("../assets/Light-Cover-Pattern-bg@2x.png");
    background-size: 70%;
  }
  .fila1 {
    height: 40px;
    border: solid black 1px;
  }

  #img1 {
    height: 24px;
    width: 24px;
    margin-left: 15px;
    /* margin-bottom: 5px; */
  }
  .c1 {
    text-align: left;
  }
  .span1 {
    display: inline;

    font-family: Nexa-XBold;
    font-size: 14px;
    color: #3b3b3b;
    text-align: center;
    line-height: 12px;
  }
  .c {
    text-align: right;
  }
  .span2 {
    display: inline-block;
    letter-spacing: 1px;

    /* width:  95px;
    height: 14px; */

    font-family: Nexa-XBold;
    font-size: 12px;
    color: #3b3b3b;
    text-align: center;
    line-height: 13px;

    text-decoration: underline #3b3b3b;
  }

  #img2 {
    height: 27px;
    width: 27px;
    margin-right: 15px;
  }
  .fila2 {
    border: solid black 1px;
    justify-content: center;
  }
  #logogrande {
    margin-left: 19px;
    margin-top: 24px;
    margin-bottom: 5px;
    height: 30px;
    width: 223px;
  }
  .fila3 {
    border: solid black 1px;
    justify-content: center;
    height: 75px;
  }
  #login {
    margin-top: 40px;
    font-family: Nexa-XBold;
    font-size: 25px;
    color: #1a1b1c;
    letter-spacing: 1px;
    text-align: center;
    line-height: 30px;
  }
  .fila4 {
    border: solid black 1px;
    justify-content: center;
  }
  #accede {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #84868a;
    letter-spacing: 0;
    text-align: center;
    line-height: 20px;
  }
  .fila5 {
    border: solid black 1px;
    justify-content: space-around;
    height: 20px;
    margin-top: 15px;
  }
  #letrasacceso {
    font-family: Nexa-Bold;
    font-size: 12px;
    color: #3b3b3b;
    text-align: center;
    line-height: 12px;
  }
  .hr {
    width: 33px;
    margin: 5px;
    background: #9ea0a4;
    margin-right: 5px;
    margin-left: 5px;
    margin-top: 9px;
  }
  .fila6 {
    justify-content: center;
    border: solid black 1px;
  }
  .fila6-1,
  .fila6-2 {
    border: solid black;
    margin-right: 5px;
  }

  .fila6-3 {
    border: solid black;
  }
  .iconosredes {
    margin-left: 0px;
    margin-top: 23px;
    cursor: pointer;
  }
  #face {
    margin-right: 15px;
  }
  .fila7 {
    border: solid black 1px;
    justify-content: space-around;
    height: 20px;
    margin-top: 28px;
  }
  .hr2 {
    width: 43px;
    margin-top: 9px;
    background: #9ea0a4;
  }
  .fila8 {
    border: solid black 1px;
    height: 80px;
    margin-top: 20px;
  }
  .fila8-1 {
    border: solid black 1px;
    margin-left: 20px;
  }
  #emailregistro {
    margin-bottom: 6px;
    font-family: Lato-Regular;
    font-size: 13px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 13px;
  }
  #casillaemail {
    height: 45px;
    width: 99%;
  }

  .fila9 {
    border: solid black 1px;
    height: 80px;
    margin-top: 0px;
  }

  .fila10 {
    height: 35px;
    border: solid black 1px;
  }
  .fila10-1 {
    border: solid black 1px;
    padding: 0%;
    display: flex;
    /* justify-content: start; */
  }
  .fila10-2 {
    border: solid black 1px;
    display: flex;
    justify-content: flex-end;
    padding: 0%;
  }
  #textocheck {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 20px;
    margin-bottom: 0px;
    position: relative;
  }
  #letrascontra {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #fa2398;
    letter-spacing: 0;
    text-align: right;
    line-height: 20px;
    margin-top: 7px;
    margin-right: 20px;
  }

  .fila11 {
    border: solid black 1px;
  }
  .fila11-1 {
    border: solid black 1px;
    display: flex;
    justify-content: center;
    padding: 0%;
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

  .contenedorPrincipal {
    height: 694px;
    width: 409px;
    background-color: white;
    position: relative;
    margin-top: 100px;
    border-radius: 1%;
    margin-bottom: 100px;
  }
  .contenedorImagen {
    background-image: url("../assets/Light-Cover-Pattern-bg@2x.png");
    background-size: 70%;
  }
  .fila1 {
    height: 40px;
    margin-top: 10px;
    border: solid black 1px;
  }

  #img1 {
    height: 24px;
    width: 24px;
    margin-left: 15px;
    /* margin-bottom: 5px; */
  }
  .c1 {
    text-align: left;
  }
  .span1 {
    display: inline;

    font-family: Nexa-XBold;
    font-size: 14px;
    color: #3b3b3b;
    text-align: center;
    line-height: 12px;
  }
  .c {
    text-align: right;
  }
  .span2 {
    display: inline-block;
    letter-spacing: 1px;

    /* width:  95px;
    height: 14px; */

    font-family: Nexa-XBold;
    font-size: 12px;
    color: #3b3b3b;
    text-align: center;
    line-height: 13px;

    text-decoration: underline #3b3b3b;
  }

  #img2 {
    height: 27px;
    width: 27px;
    margin-right: 15px;
  }
  .fila2 {
    border: solid black 1px;
    justify-content: center;
  }
  #logogrande {
    margin-left: 19px;
    margin-top: 24px;
    margin-bottom: 5px;
    height: 30px;
    width: 223px;
  }
  .fila3 {
    border: solid black 1px;
    justify-content: center;
    height: 75px;
    margin-top: 10px;
  }
  #login {
    margin-top: 37px;
    font-family: Nexa-XBold;
    font-size: 25px;
    color: #1a1b1c;
    letter-spacing: 1px;
    text-align: center;
    line-height: 30px;
  }
  .fila4 {
    border: solid black 1px;
    justify-content: center;
  }
  #accede {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #84868a;
    letter-spacing: 0;
    text-align: center;
    line-height: 20px;
  }
  .fila5 {
    border: solid black 1px;
    justify-content: space-around;
    height: 20px;
    margin-top: 15px;
  }
  #letrasacceso {
    font-family: Nexa-Bold;
    font-size: 12px;
    color: #3b3b3b;
    text-align: center;
    line-height: 12px;
  }
  .hr {
    width: 33px;
    margin: 5px;
    background: #9ea0a4;
    margin-right: 5px;
    margin-left: 5px;
    margin-top: 9px;
  }
  .fila6 {
    justify-content: center;
    border: solid black 1px;
  }
  .fila6-1,
  .fila6-2 {
    border: solid black;
    margin-right: 5px;
  }

  .fila6-3 {
    border: solid black;
  }
  .iconosredes {
    margin-left: 0px;
    margin-top: 23px;
    cursor: pointer;
  }
  #face {
    margin-right: 15px;
  }
  .fila7 {
    border: solid black 1px;
    justify-content: space-around;
    height: 20px;
    margin-top: 28px;
  }
  .hr2 {
    width: 43px;
    margin-top: 9px;
    background: #9ea0a4;
  }
  .fila8 {
    border: solid black 1px;
    height: 80px;
    margin-top: 20px;
  }
  .fila8-1 {
    border: solid black 1px;
    margin-left: 35px;
  }
  #emailregistro {
    margin-bottom: 6px;
    font-family: Lato-Regular;
    font-size: 13px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 13px;
  }
  #casillaemail {
    height: 45px;
    width: 90%;
  }

  .fila9 {
    border: solid black 1px;
    height: 80px;
    margin-top: 0px;
  }

  .fila10 {
    height: 35px;
    border: solid black 1px;
  }
  .fila10-1 {
    border: solid black 1px;
    padding: 0%;
    display: flex;
    /* justify-content: start; */
  }
  .fila10-2 {
    border: solid black 1px;
    display: flex;
    justify-content: flex-end;
    padding: 0%;
  }
  #textocheck {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 20px;
    margin-bottom: 0px;
    position: relative;
  }
  .custom-radio-checkbox__input {
    margin-left: 0px;
  }
  #letrascontra {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #fa2398;
    letter-spacing: 0;
    text-align: right;
    line-height: 20px;
    margin-top: 7px;
    margin-right: 12px;
  }

  .fila11 {
    border: solid black 1px;
  }
  .fila11-1 {
    border: solid black 1px;
    display: flex;
    justify-content: center;
    padding: 0%;
  }
}
</style>
