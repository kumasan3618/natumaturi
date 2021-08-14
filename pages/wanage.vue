<template>
  <v-container>
    <v-card class="pa-4">
      <h1>輪 投 げ</h1>
      <div class="card_text">
        <p>輪を投げて棒に入れよう</p>
      </div>
      <v-card-title class="pt-0">操作方法</v-card-title>
      <p>使うボタンは五つ！(A,W,S,D,spacekey)</p>
      <li>A：銃口が左に向くよ！</li>
      <li>W：銃口が上に向くよ！</li>
      <li>S：銃口が右に向くよ！</li>
      <li>D：銃口が下に向くよ！</li>
      <li>spacekey：弾丸を打って的に当てよう！</li>
    </v-card>
    <iframe
      width="100%"
      height="750px"
      src="https://daipengin.github.io/syateki2/"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </v-container>
</template>

<style>
.syateki_title {
  display: flex;
  justify-content: center;
  align-items: center;
}
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
