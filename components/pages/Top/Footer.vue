<template>
  <div class="l-footer">
    <div class="container">
      <a class="enactment">制定:2019.01.01</a>
    </div>
  </div>
</template>



<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .l-footer {
    height:90px;
    background: #ba3a32;

    .container {
      width: 926px;
      margin: 0 auto;
      color: white;
      letter-spacing: 1px;
      text-align: center;

      .enactment{
        display:inline-block;
        margin-top: 33px;
        font-size:1.3rem;
      }
    }
  }
</style>
