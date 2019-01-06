<template>
  <div class="l-header">
    <div class="container">
        <a class="company-name">chatbox</a>
      </div>
    </div>
</template>



<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .l-header {
    height:60px;
    background: #ba3a32;

    .container {
      width: 926px;
      margin: 0 auto;
      color: white;
      letter-spacing: 1px;
      text-align: right;

      .company-name{
        display:inline-block;
        margin-top: 5px;
       font-size:30px;
        font-weight: bold;
      }
    }
  }
</style>
