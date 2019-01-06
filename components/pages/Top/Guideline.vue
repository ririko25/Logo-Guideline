<template>
  <div class="box">
   <div class="c-container">
    <br>
    <div class="md-body">
      <div class="m-container" v-html="bodyHtml">
      </div>
    </div>
     </div>
    <br>
  </div>
</template>

<script>
export default {
  props:["title", "bodyHtml"],
}
</script>


<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .box{
    background-color:#f2f3f4;
  }

  .post-meta {
    font-size: 0.8em;
    color: #888;
    margin-top: -1rem;
    margin-bottom: 2.4rem;
    text-align: right;
  }


  h1{
    color:#707070;
  }

  .md-body {
    border-radius:10px;
    margin-top:40px;
    margin-bottom:160px;
    background-color: #fff;
    /deep/.m-container  {
      margin: 0 auto;
      padding:0 20px 75px 20px ;
      width: 100%;
      max-width: 845px;
      box-sizing: border-box;
      /deep/ h1 {
           display: inline-block;
           margin-top: 35px;
           padding-left: 5px;
           color: #707070;
           font-size:2.4rem;
           font-weight:bold;
           border-left:0.4rem solid #ba3a32;
         }
      /deep/ h2 {
        padding-top:40px;
        padding-bottom:10px;
        color: #707070;
        font-size:1.6rem;
        font-weight:bold;
      }
      /deep/ p {
        color: #707070;
        font-size: 1.3rem;
      }
      /deep/ li {
        color: #707070;
        font-size: 1.3rem;
      }
      /deep/ img{
        padding:50px 50px 30px 50px;

      }
      /deep/ td{
        color: #707070;
        font-size: 1.3rem;
        text-align: center;
        /*width: 100%;*/
        /*display: block;*/
      }
      /*/deep/ th{*/
        /*width: 100%;*/
        /*display: block;*/
      /*}*/
    }
  }

  /deep/.img{
    display:flex;
  }
  /deep/.banimg{
    text-align:center;
  }


</style>
