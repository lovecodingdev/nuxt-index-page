<template>
  <div class="tab-content" :class="{'relative': !active, 'active': active}">
    <div class="tab-title">{{title}}</div>
    <div class="step-1 relative">
      <div class="image absolute" :style="step_img(0)"></div>
      <span class="no absolute">{{steps[0].id}}.</span>
      <span class="desc absolute">{{steps[0].desc}}</span>
    </div>
    <div class="step-2-wrapper relative">
      <svg class="svg-top" viewBox="0 0 500 500" preserveAspectRatio="none">
        <path d="M0,160 L500,160 L500,00 C150,200 350,0 0,0 Z" style="stroke: none; fill:#E6FFFA;"></path>
      </svg>
      <div class="step-2 relative">
        <span class="no absolute">{{steps[1].id}}.</span>
        <span class="desc absolute">{{steps[1].desc}}</span>
        <div class="image absolute" :style="step_img(1)"></div>
      </div>
      <svg class="svg-down" viewBox="0 0 500 500" preserveAspectRatio="none">
        <path d="M0,160 C50,100 250,50 500,100 L500,00 L0,0 Z" style="stroke: none; fill:#E6FFFA;"></path>
      </svg>
    </div>
    <div class="step-3 relative">
      <span class="no absolute">{{steps[2].id}}.</span>
      <span class="desc absolute">{{steps[2].desc}}</span>
      <div class="image absolute" :style="step_img(2)"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['active', 'title', 'steps'],
  methods: {
    step_img(step) {
      return `background: transparent url('${this.steps[step].img}') right top no-repeat padding-box;`
    }
  }
}
</script>

<style lang="scss" scoped>
.tab-content {
  position: relative;
  display: none;
  width: 360px;
  opacity: 1;
}

.active {
  display: block;
}

.tab-title{
  left: 40px;
  width: 280px;
  height: 50px;
  text-align: center;
  font: normal normal 500 21px/25px 'Lato Medium';
  letter-spacing: 0px;
  color: #4A5568;
  margin: 20px auto;
  opacity: 1;
}

.step-1 {
  padding-left: 0px;
  width: 354px;
  height: 265px;
  opacity: 1;
  .image {
    height: 145px;
    opacity: 1;
  }
  .no {
    bottom: 20px;
  }
  .desc {
    bottom: 50px;
    left: 120px;
  }
}
.step-2 {
  padding-left: 25px;
  width: 354px;
  height: 282px;
  opacity: 1;
  background: #E6FFFA;
  .image {
    bottom: 0px;
    height: 179px;
    opacity: 1;
  }
  .no {
    top: 0px;
  }
  .desc {
    bottom: 155px;
    left: 145px;
  }
}
.step-3 {
  padding-left: 50px;
  width: 354px;
  height: 370px;
  opacity: 1;
  .image {
    bottom: 0px;
    height: 210px;
    opacity: 1;
  }
  .no {
    top: 0px;
  }
  .desc {
    top: 60px;
    left: 175px;
  }
}

.step-2-wrapper{
  .svg-top {
    top:-20px;
    width: 100%;
    height: 150px;
    position: absolute;
  }
  .svg-down {
    width: 100%;
    height: 150px;
    position: absolute;
  }
}

.no {
  width: 106px;
  height: 156px;
  text-align: center;
  font: normal normal normal 130px/156px 'Lato Regular';
  letter-spacing: 0px;
  color: #718096;
  opacity: 1;
  z-index: 30;
}

.desc {
  text-align: left;
  font: normal normal normal 16px 'Lato Regular';
  letter-spacing: 0.47px;
  color: #718096;
  opacity: 1;
  z-index: 30;
}

.image {
  z-index: 30;
  width: 100%;
  right: 20px;
}

</style>