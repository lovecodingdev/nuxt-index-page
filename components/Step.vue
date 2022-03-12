<template>
  <div class="step relative">
    <div class="step-img" :style="background"></div>
    <span class="step-no absolute">{{no}}.</span>
    <span class="step-content absolute">{{content}}</span>
  </div>
</template>

<script>
export default {
  props: ['no', 'content', 'img', 'top', 'ibottom'],
  computed: {
    background() {
      return `background: transparent url('${this.img}') right no-repeat padding-box;`
    }
  }
}
</script>

<style>
.step {
  /* left: -34px; */
  width: 354px;
  height: 265px;

  margin: 0px auto;
  opacity: 1;
}

.step-img {
  /* top: 851px; */
  right: 20px;
  width: 220px;
  height: 145px;
  background-position: right;
  opacity: 1;
}

.step-no {
  bottom: 20px;
  left: 10px;
  width: 106px;
  text-align: center;

  font: normal normal normal 130px/130px 'Lato Regular';
  letter-spacing: 0px;
  color: #718096;
  opacity: 1;
  z-index: 30;
}

.step-content {
  bottom: 36px;
  left: 137px;
}
</style>