<script setup>

</script>

<template>
  <main>
      <div class="layer">
      <div>
          <img :src='`https://cdn.pixabay.com/photo/2015/09/13/20/32/checks-938700_1280.jpg`' alt=""/>
      </div>
          
          <div>
              <b>
                  <span> 영화를 스트리밍 중이신가요? </span>
                </b>
          </div>
          <div style="margin: 900px 20px 30px 1100px;">
              <a style="display: inline-block" href="#">
                  <span class="click">네</span>
              </a>
              <a style="display: inline-block" href="#">
                  <span class="click">아니요</span>
              </a>


          </div>

      </div>
  </main>

</template>

<style scoped>
main {
    position: relative;
    height: 100%;
    width: 100%;
}
.layer {
    position: absolute;
    width: auto;
    height: 100%;
    top: 0;
    left: 0;
    background: #333333;
    display: block;
    padding: 20px;
}
img{
    width: 100px;
    height: 100px;
}
b{
    position: absolute;
    font-size: 40px;
    color: white;
    top: 450px;
    left: 500px;
    padding: 20px 20px 20px 20px;
}

.layer .click {
    margin-right: 10px;
    padding: 10px 50px 10px 50px ;
    color: white;
    background-color: gray;
}



</style>