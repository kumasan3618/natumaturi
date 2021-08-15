<template>
  <v-container>
    <v-card class="pa-4">
      <h1>輪 投 げ</h1>
      <div class="card_text">
        <p>輪を投げて棒に入れよう</p>
      </div>
      <v-card-title class="pt-0">操作方法</v-card-title>
      <p>使うボタンは1つ！(spacekey)</p>
      <li>spacekey:1回目は輪が出てきて左右に動くよ！</li>
      <li>spacekey:2回目は上下に動くよ！</li>
      <li>spacekey:3回目は場所が決定し輪を投げるよ！</li>
    </v-card>
    <iframe
      width="100%"
      height="750px"
      src="https://daipengin.github.io/wanage2/"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </v-container>
</template>

<style>
h1 {
  font-size: 60px;
  color:blue;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 3px 3px 0 #000,
               -1px 1px 0 #fff;
  padding:1rem;
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
}
</style>
