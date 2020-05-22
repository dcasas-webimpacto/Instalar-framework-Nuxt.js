<template>
  <button type="button" class="btn btn-primary btn-block">{{contenido}}</button>
</template>

<script>
export default {
  props: ["contenido"]
};
</script>

<style scoped>
button {
  background-color: #fa2398;
  border-color: #fa2398;
  color: #ffffff;
}
.btn-primary:hover {
  color: #fff;
  background-color: #f10586;
  border-color: #e5057f;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #f10586;
  border-color: #e5057f;
  box-shadow: 0 0 0 0.2rem rgba(251, 68, 167, 0.5);
}
.btn-primary.disabled,
.btn-primary:disabled {
  color: #fff;
  background-color: #fa2398;
  border-color: #fa2398;
}
.btn-primary:not(:disabled):not(.disabled):active,
.btn-primary:not(:disabled):not(.disabled).active,
.show > .btn-primary.dropdown-toggle {
  color: #fff;
  background-color: #e5057f;
  border-color: #d80578;
}
.btn-primary:not(:disabled):not(.disabled):active:focus,
.btn-primary:not(:disabled):not(.disabled).active:focus,
.show > .btn-primary.dropdown-toggle:focus {
  box-shadow: 0 0 0 0.2rem rgba(251, 68, 167, 0.5);
}
</style>