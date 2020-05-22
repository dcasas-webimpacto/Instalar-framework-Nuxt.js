<template>
  <label class="custom-radio-checkbox">
    <label class="checkbox" id="checknews" @click="cambiacheck"></label>
    <span
      class="custom-radio-checkbox__show custom-radio-checkbox__show--checkbox"
      id="textocheck"
      >Recuérdame</span
    >
  </label>
</template>

<script>
export default {
  methods: {
    cambiacheck() {
      var checkk = document.getElementById("checknews");
      if (checkk.className == "checked") {
        checkk.setAttribute("class", "checkbox");
      } else {
        checkk.setAttribute("class", "checked");
      }
      //   console.log(checkk);
    }
  }
};
</script>
<style scoped>
.checkbox {
  width: 18px;
  height: 18px;
  margin-top: 6px;
  margin-bottom: 0px;
  border: 1px solid #c0c2c8;
}
.checked {
  width: 18px;
  height: 18px;
  margin-top: 6px;
  margin-bottom: 0px;
  background: url("~assets/check.svg") no-repeat 30% 60%;
  border: solid black 1px;
}
@media (max-width: 766px) {
  .checkbox {
    margin-left: 17px;
  }
  .checked {
    margin-left: 17px;
  }
  #textocheck {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 20px;
    margin-bottom: 10px;
  }
  label.custom-radio-checkbox {
    margin-bottom: 10px;
  }
}
@media (min-width: 766px) {
  #textocheck {
    font-family: Lato-Regular;
    font-size: 14px;
    color: #3b3b3b;
    letter-spacing: 0;
    line-height: 20px;
    margin-bottom: 10px;
  }
  label.custom-radio-checkbox {
    margin-bottom: 10px;
  }
}
</style>
