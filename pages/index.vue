<template>
  <v-container>
    <v-card class="pa-4">
      <h1>夏祭り屋台ミニゲーム</h1>
    <div class="card_text">
      <p>夏祭りの屋台ゲームが盛りだくさん！</p>
    </div>
    <div class="card_title_description">
      <v-card-title class="font-weight-medium">四つのゲームでスコアを稼ごう</v-card-title>
    </div>
    </v-card>
    <div class="minigame">
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12 sl2>
          <v-layout justify-content:center>
            <v-card class="pa-4">
              <h2 class="yatai_title">金魚すくい</h2>
              <div class="card_text">
                <p>金魚をねらってすくってみよう。ゲットするとポイントがもらえるよ！</p>
              </div>
              <p>
              <a href="/kingyo">
                <img src="https://3.bp.blogspot.com/-7RdvF7W1rQ4/VKTgoGDmVsI/AAAAAAAAqVk/pgragsSDFGI/s180-c/pyoko08_kingyosukui.png">
                  <v-btn outlline rounded class="blue lighten-3">金魚すくいへ</v-btn>
              </a>
              </p>
            </v-card>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <v-card class="pa-4">
              <h2 class="yatai_title">射的</h2>
              <div class="card_text">
                <p>撃つものごとにポイントが変わるよ！　　　　　　　　　　　　　　　</p>
              </div>
              <a href="/syateki">
              <p>
                <img src="http://3.bp.blogspot.com/-uMiiSsDjRh4/UZM5GkVfQeI/AAAAAAAASTc/pySNdfZiMG8/s180-c/omatsuri_syateki.png">
                <v-btn outlline rounded class="blue lighten-3">射的ゲームへ</v-btn>
              </p>
              </a>
              
            </v-card>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <v-card class="pa-4">
              <h2 class="yatai_title">輪投げ</h2>
              <div class="card_text">
                <p>入れる場所によってポイントが変わるよ！　　　　　　　　　　　　　</p>
              </div>
              <p>
              <a href="/wanage">
                <img src="https://1.bp.blogspot.com/-Dmb6PNjwanE/XZR98B9i9fI/AAAAAAABVXI/q6p7bR4kDv4ek0cE4VchXJPVEodphTwDwCNcBGAsYHQ/s180-c/sports_wanage_board_wa.png">
                <v-btn outlline rounded class="blue lighten-3">輪投げゲームへ</v-btn>
              </a>
              </p>
            </v-card>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <v-card class="pa-4">
              <h2 class="yatai_title">ポイント交換所</h2>
              <div class="card_text">
                <p>集めたポイントと景品を交換しよう！　　　　　　　　　　　　　　　</p>
              </div>
              <p>
              <a href="/koukan">
                <img src="https://4.bp.blogspot.com/-_iHoiU4-aYg/Wat2Uk9FoVI/AAAAAAABGW8/cdVzb2nDlZsNthMbmEv6Xhw-UKErrxZVACLcBGAs/s180-c/building_pachinko_keihin_koukanjo.png">
                <v-btn outlline rounded class="blue lighten-3">交換所へ</v-btn>
              </a>
              </p>
            </v-card>
          </v-layout>
        </v-flex>
      </v-layout>
    </div>
  </v-container>
</template>

<style>
*{
  float:none;
  position:static
}
.card_text{
  font-size: 16px;
  display: flex;
  justify-content:center;
  align-items:center;
}
h1{
  font-size: 60px;
  color: blue;
  background-color: rgb(52, 241, 185);
  display: flex;
  justify-content:center;
  align-items:center;
}
h2{
  color: blue;
  display: flex;
  justify-content:center;
  align-items:center;
}
.card_title_description{
  color: rgb(255, 8, 0);
  font-size: 40px;
  display: flex;
  justify-content:center;
  align-items:center;
}
.minigame{
  display:flex;
  flex-flow: row wrap;
}
a{
  text-decoration: none;
}
.yatai_title{
  display: flex;
  justify-content:center;
  flex-direction: column;
  align-items:center;
}

</style>