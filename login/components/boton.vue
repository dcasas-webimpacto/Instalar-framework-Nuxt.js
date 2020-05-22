<template>
  <button
    type="button"
    class="btn btn-primary btn-lg btn-block"
    id="botonregistro"
  >
    Iniciar sesión
  </button>
</template>

<script>
export default {
  name: "botonreg"
};
</script>

<style scoped>
@font-face {
  font-family: "Nexa-Xbold";
  src: url("~static/Nexa/Nexa_V1_2012/Nexa\ Bold.otf");
}
@media (max-width: 766px) {
  #botonregistro {
    font-family: Nexa-XBold;
    font-size: 16px;
    color: #ffffff;
    letter-spacing: 0;
    text-align: center;
    line-height: 15px;
    width: 77%;
    height: 70%;
  }
  .btn {
    width: 85%;
    height: 50%;
    margin-bottom: 15px;
    background-color: #fa2398;
    border-color: #fa2398;
    margin-top: 8px;
    border-radius: 4px;
  }
}
@media (min-width: 766px) {
  #botonregistro {
    width: 77%;
    height: 70%;
    margin-bottom: 15px;
    background-color: #fa2398;
    border-color: #fa2398;
    margin-top: 8px;
    border-radius: 4px;
    font-family: Nexa-XBold;
    font-size: 16px;
    color: #ffffff;
    letter-spacing: 0;
    text-align: center;
    line-height: 15px;
  }
}
</style>
