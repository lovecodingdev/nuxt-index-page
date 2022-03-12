<template>
  <div>
    <div class="color-bar fixed z-40"></div>
    <div class="login-card fixed z-40">
      <button class="login-btn absolute">Login</button>
    </div>
  </div>
</template>

<style scoped>
.color-bar {
  /* Layout Properties */
  top: 0px;
  width: 100%;
  height: 5px;

  /* UI Properties */
  background: transparent linear-gradient(91deg, #319795 0%, #3182ce 100%) 0% 0%
      no-repeat padding-box;
  opacity: 1;
}

.login-card {
  /* Layout Properties */
  top: 5px;
  left: 0px;
  width: 100%;
  height: 67px;

  /* UI Properties */
  background: #FFFFFF 0% 0% no-repeat padding-box;
  box-shadow: 0px 3px 6px #00000029;
  border-radius: 0px 0px 12px 12px;
  opacity: 1;
}

.login-btn {
  /* Layout Properties */
  top: 26px;
  right: 20px;

  /* UI Properties */
  text-align: left;
  font: normal normal 600 13px/17px 'Lato';
  letter-spacing: 0.84px;
  color: #319795;
  opacity: 1;
}
</style>