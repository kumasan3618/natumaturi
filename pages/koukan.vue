<template>
  <v-container>
    <v-card class="pa-4">
      <h1>交換所</h1>
      <div class="card_text">
        <p>結果発表</p>
      </div>
      <v-card-title class="pt-0">各結果</v-card-title>
      <ol>
      <li>金魚すくい:</li>
      <li>射的:</li>
      <li>輪投げ:</li>
    </ol>
      <v-card-title class="pt-0">最終結果:</v-card-title>
    </v-card>
    
    <p id="kekka"></p>
  </v-container>
</template>

<style>
h1 {
  font-size: 60px;
  color:blue;
  background-color: rgb(52, 241, 185);
  display: flex;
  justify-content: center;
  align-items: center;
}
.card_text{
  font-size: 16px;
  display: flex;
  justify-content:center;
  align-items:center;
  padding-top:1% ;
}
</style>