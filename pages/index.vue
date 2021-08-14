<template>
  <v-container>
    <v-card class="pa-4">
    <v-card-title class="font-weight-bold green lighten-2">夏祭り屋台ミニゲーム</v-card-title>
    <v-card-text>夏祭りの屋台ゲームが盛りだくさん！</v-card-text>
    <div class="card_title">
      <v-card-title class="font-weight-medium">四つのゲームでスコアを稼ごう</v-card-title>
    </div>
    </v-card>
    <div class="minigame">
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12 sl2>
          <v-layout justify-content:center>
            <v-card class="pa-4">
              <div class="item">
              <v-card-title class="font-weight-bold">金魚すくい</v-card-title>
              </div>
              <v-card-text>金魚をねらってすくってみよう。ゲットするとポイントがもらえるよ！</v-card-text>
              <p>
              <a href="/kingyo">
                <img src="https://3.bp.blogspot.com/-7RdvF7W1rQ4/VKTgoGDmVsI/AAAAAAAAqVk/pgragsSDFGI/s180-c/pyoko08_kingyosukui.png">
                  <v-btn outlline round class="blue lighten-3">金魚すくいへ</v-btn>
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
              <div class="item">
              <v-card-title class="font-weight-bold">射的</v-card-title>
              </div>
              <v-card-text>撃つものごとにポイントが変わるよ！　　　　　　　　　　　　　　　</v-card-text>
              <a href="/syateki">
              <p>
                <img src="http://3.bp.blogspot.com/-uMiiSsDjRh4/UZM5GkVfQeI/AAAAAAAASTc/pySNdfZiMG8/s180-c/omatsuri_syateki.png">
                <v-btn outlline round class="blue lighten-3">射的ゲームへ</v-btn>
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
              <div class="item">
              <v-card-title class="font-weight-bold">輪投げ</v-card-title>
              </div>
              <v-card-text>入れる場所によってポイントが変わるよ！　　　　　　　　　　　　　</v-card-text>
              <p>
              <a href="/wanage">
                <img src="https://1.bp.blogspot.com/-Dmb6PNjwanE/XZR98B9i9fI/AAAAAAABVXI/q6p7bR4kDv4ek0cE4VchXJPVEodphTwDwCNcBGAsYHQ/s180-c/sports_wanage_board_wa.png">
                <v-btn outlline round class="blue lighten-3">輪投げゲームへ</v-btn>
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
              <div class="item">
              <v-card-title class="font-weight-bold">ポイント交換所</v-card-title>
              </div>
              <v-card-text>集めたポイントと景品を交換しよう！　　　　　　　　　　　　　　　</v-card-text>
              <p>
              <a href="/koukan">
                <img src="https://4.bp.blogspot.com/-_iHoiU4-aYg/Wat2Uk9FoVI/AAAAAAABGW8/cdVzb2nDlZsNthMbmEv6Xhw-UKErrxZVACLcBGAs/s180-c/building_pachinko_keihin_koukanjo.png">
                <v-btn outlline round class="blue lighten-3">交換所へ</v-btn>
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
.card_title{
  color: cornflowerblue;
}
.minigame{
  display:flex;
  flex-flow: row wrap;
}
a{
  text-decoration: none;
}
.item{
  display: flex;
  justify-content:center;
  flex-direction: column;
  align-items:center;
}

</style>