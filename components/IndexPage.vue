<template>
  <div class="board">
    <Header/>
    <div class="background">
      <div class="heading-text">Deine Job website</div>
      <div class="undraw-agreement curved-div"></div>
      <svg viewBox="0 0 500 500" preserveAspectRatio="none">
        <path d="M0,160 C150,200 350,0 500,100 L500,00 L0,0 Z" style="stroke: none; fill:#E6FFFA;"></path>
      </svg>
    </div>
    <Tabs/>
    <Footer/>
  </div>
</template>

<style lang="scss">
.board {
  padding-bottom: 90px;
}

.background {
  padding-top: 90px;
  /* Layout Properties */
  top: 0px;
  width: 100%;
  height: 600px;

  /* UI Properties */
  background: transparent linear-gradient(141deg, #EBF4FF 0%, #E6FFFA 100%) 0% 0% no-repeat padding-box;
  opacity: 1;

  svg {
    width: 100%;
    height: 150px;
  }
}

.heading-text {
  /* Layout Properties */
  top: 90px;
  height: 100px;

  /* UI Properties */
  margin: 0px 20px;
  text-align: center;
  font: normal normal 500 42px/50px 'Lato';
  letter-spacing: 1.26px;
  color: #2D3748;
  opacity: 1;
}

.undraw-agreement {
  /* Layout Properties */
  width: 100%;
  height: 400px;

  /* UI Properties */
  background: transparent url('/img/undraw_agreement_aajr.svg') 0% 0% no-repeat padding-box;
  background-size: cover;
  opacity: 1;
}

</style>