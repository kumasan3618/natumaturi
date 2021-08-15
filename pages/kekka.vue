<template>
  <v-container>
    <v-card class="pa-4">
      <h1 class="kekka_title">結果</h1>
      <div class="card_text">
        <h3>結果発表</h3>
      </div>
      <div class="kakukekka">
      <v-card-title class="pt-0">各結果</v-card-title>
      <ol>
        <li>金魚すくい:<span>300点</span></li>
        <li>射的:<span>100点</span></li>
        <li>輪投げ:<span>250点</span></li>
      </ol>
      </div>
      <v-card-title class="pt-0"><h4>最終結果:<span>650点</span></h4></v-card-title>
    </v-card>
    
    <p id="kekka"></p>
  </v-container>
</template>

<style>

.kekka_title {
  font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro', 'Hiragino Mincho ProN', 'HGS明朝E', 'ＭＳ Ｐ明朝', serif;
  position: relative;
  padding: 1.5rem 2rem;
  -webkit-box-shadow: 0 2px 14px rgba(0, 0, 0, .1);
  box-shadow: 0 2px 14px rgba(0, 0, 0, .1);
  font-size: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 1px 1px 0 #000,
               -1px 1px 0 #000,
               1px -1px 0 #000,
               -1px -1px 0 #000;
}
.kekka_title:before,
.kekka_title:after {
  position: absolute;
  left: 0;
  width: 100%;
  height: 4px;
  content: '';
  background-image: -webkit-linear-gradient(315deg, #704308 0%, #ffce08 40%, #e1ce08 60%, #704308 100%);
  background-image: linear-gradient(135deg, #704308 0%, #ffce08 40%, #e1ce08 60%, #704308 100%);
}

.kekka_title:before {
  top: 0;
}

.kekka_title:after {
  bottom: 0;
}
.card_text{
  font-size: 16px;
  display: flex;
  justify-content:center;
  align-items:center;
  padding-top:1% ;
  font-size:2rem;
}
.kakukekka{
  display: flex;
  justify-content:flex-start;
  align-items:center;
  padding-bottom: 10px;
}
ol li span{
  color:red;
}
h4{
  display: flex;
  justify-content:center;
  align-items:center;
}
h4 span{
  font-size: 30px;
  color:crimson
}
</style>