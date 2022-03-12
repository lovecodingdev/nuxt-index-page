<template>
  <div class="button-nav-bg fixed z-40">
    <button class="button-primary relative">
        <span class="text-primary">Kostenlos Registrieren</span>
    </button>
  </div>
</template>

<style scoped>
.button-nav-bg {
  bottom: 0px;
  width: 100%;
  height: 88px;

  background: #FFFFFF 0% 0% no-repeat padding-box;
  box-shadow: 0px -1px 3px #00000033;
  border-radius: 12px 12px 0px 0px;
  opacity: 1;
}

.button-primary {
  top: 24px;
  left: 20.02px;
  width: calc( 100% - 40px );
  height: 40px;

  background: transparent linear-gradient(95deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
  border-radius: 12px;
  opacity: 1;
}

.text-primary {
  top: 12px;
  left: 20px;
  width: 320px;
  height: 17px;

  text-align: center;
  font: normal normal 500 14px/17px 'Lato Light';
  letter-spacing: 0.84px;
  color: #E6FFFA;
  opacity: 1;
}

</style>