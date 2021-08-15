<template>
  <v-container>
    <v-card class="pa-4">
      <h1 class="kingyo_title">ボールすくい</h1>
      <div class="card_text">
        <p>ボールをいっぱいすくおう</p>
      </div>
      <v-card-title class="pt-0">操作方法</v-card-title>
      <p>ただいま準備中</p>
    </v-card>
    <iframe
      width="100%"
      height="750px"
      src="https://daipengin.github.io/tamasukui2/"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </v-container>
</template>

<style>
.kingyo_title {
  font-size: 60px;
  color:deepskyblue;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 3px 3px 0 #000,
               -1px 1px 0 #fff;
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
