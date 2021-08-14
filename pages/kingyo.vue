<template>
  <v-container>
    <v-card class="pa-4">
      <h1 class="kingyo_title">金魚すくい</h1>
      <div class="card_text">
        <p>金魚をいっぱいすくおう</p>
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
.kingyo_title {
  font-size: 60px;
  color: blue;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 1px 1px 0 #000,
               -1px 1px 0 #000,
               1px -1px 0 #000,
               -1px -1px 0 #000;
  padding: 1rem 3rem;
  border-radius: 10vh;
  background-image: -webkit-gradient(linear, right top, left top, from(#9be15d), to(#00e3ae));
  background-image: -webkit-linear-gradient(right, #9be15d 0%, #00e3ae 100%);
  background-image: linear-gradient(to left, #9be15d 0%, #00e3ae 100%);
}

.card_text{
  font-size: 16px;
  display: flex;
  justify-content:center;
  align-items:center;
  padding-top:1% ;
  padding-bottom: 0;
}
</style>
