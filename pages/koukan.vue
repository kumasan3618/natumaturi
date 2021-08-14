<template>
  <v-container>
    <v-card class="pa-4">
      <h1>交換所</h1>
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
h3{
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
  font-size: 2rem;
}
h1 {
  font-size: 60px;
  color:blue;
  background-color: rgb(52, 241, 185);
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 1px 1px 0 #000,
               -1px 1px 0 #000,
               1px -1px 0 #000,
               -1px -1px 0 #000;
}
.card_text{
  font-size: 16px;
  display: flex;
  justify-content:center;
  align-items:center;
  padding-top:1% ;
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