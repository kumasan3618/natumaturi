<template>
  <v-container>
    <v-card class="pa-4">
      <h1 class="card_title">夏祭り屋台ミニゲーム</h1>
      <div class="card_text">
        <p>夏祭りの屋台ゲームが盛りだくさん！</p>
      </div>
      <div class="card_title_description">
        <v-card-title class="font-weight-bold"
          >３つのゲームでスコアを稼ごう</v-card-title
        >
      </div>
    </v-card>
    <div class="minigame">
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12 sl2>
          <v-layout justify-content:center>
            <div class="card">
              <v-card class="pa-4">
                <h2 class="yatai_title">ボールすくい</h2>
                <div class="card_text">
                  <p>
                    ボールをねらってすくってみよう。
                  </p>
                </div>

                <a href="/tama">
                  <img
                    src="http://3.bp.blogspot.com/-ieWTcRTJa1s/UgsvKxNt9HI/AAAAAAAAXRc/QuRVb2K7rK4/s180-c/superball_sukui.png"
                  />
                  <v-btn
                    outlline
                    rounded
                    class="font-weight-bold blue lighten-3"
                    >ボールすくいへ</v-btn
                  >
                </a>
              </v-card>
            </div>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <div class="card">
              <v-card class="pa-4">
                <h2 class="yatai_title">射的</h2>
                <div class="card_text">
                  <p>撃つものごとにポイントが変わるよ！</p>
                </div>

                <a href="/syateki">
                  <img
                    src="http://3.bp.blogspot.com/-uMiiSsDjRh4/UZM5GkVfQeI/AAAAAAAASTc/pySNdfZiMG8/s180-c/omatsuri_syateki.png"
                  />
                  <v-btn
                    outlline
                    rounded
                    class="font-weight-bold blue lighten-3"
                    >射的ゲームへ</v-btn
                  >
                </a>
              </v-card>
            </div>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <div class="card">
              <v-card class="pa-4">
                <h2 class="yatai_title">輪投げ</h2>
                <div class="card_text">
                  <p>入れる場所によってポイントが変わるよ！</p>
                </div>

                <a href="/wanage">
                  <img
                    src="https://1.bp.blogspot.com/-Dmb6PNjwanE/XZR98B9i9fI/AAAAAAABVXI/q6p7bR4kDv4ek0cE4VchXJPVEodphTwDwCNcBGAsYHQ/s180-c/sports_wanage_board_wa.png"
                  />
                  <v-btn
                    outlline
                    rounded
                    class="font-weight-bold blue lighten-3"
                    >輪投げゲームへ</v-btn
                  >
                </a>
              </v-card>
            </div>
          </v-layout>
        </v-flex>
      </v-layout>
      <v-layout class="pt-4">
        <v-flex sm12 md12 lg12>
          <v-layout justify-content:center>
            <div class="card">
              <v-card class="pa-4">
                <h2 class="yatai_title">ポイント交換所</h2>
                <div class="card_text">
                  <p>集めたポイントと景品を交換しよう！</p>
                </div>

                <a href="/koukan">
                  <img
                    src="https://4.bp.blogspot.com/-_iHoiU4-aYg/Wat2Uk9FoVI/AAAAAAABGW8/cdVzb2nDlZsNthMbmEv6Xhw-UKErrxZVACLcBGAs/s180-c/building_pachinko_keihin_koukanjo.png"
                  />
                  <v-btn
                    outlline
                    rounded
                    class="font-weight-bold blue lighten-3"
                    >交換所へ</v-btn
                  >
                </a>
              </v-card>
            </div>
          </v-layout>
        </v-flex>
      </v-layout>
    </div>
  </v-container>
</template>

<style>
* {
  float: none;
  position: static;
}
.card {
  width: 544px;
  background-color: #fff;
}

.card_text {
  font-size: 16px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.card_title {
  font-size: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  text-shadow: 0 0 5px #fff, 0 0 15px #fff, 0 0 35px #fff;
  border-radius: 10px;
  padding: 1rem;
  background-image: -webkit-gradient(
    linear,
    left top,
    right top,
    from(rgb(184, 0, 86)),
    to(#f83600)
  );
  background-image: -webkit-linear-gradient(
    left,
    rgb(184, 0, 86) 0%,
    #f83600 100%
  );
  background-image: linear-gradient(to right, rgb(184, 0, 86) 0%, #f83600 100%);
}

h2 {
  color: blue;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 0 0 5px #fff, 0 0 15px #fff, 0 0 35px #fff;
}
.card_title_description {
  color: rgb(255, 8, 0);
  font-size: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fef81e;
  text-shadow: 1px 1px 0 #e92525, -1px -1px 0 #2ab6f1;
}
.minigame {
  display: flex;
  flex-flow: row wrap;
}
a {
  text-decoration: none;
  display: flex;
  justify-content: center;
  align-items: center;
}
.yatai_title {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
a .v-btn {
  text-shadow: 1px 1px 0 #2ab6f1, -1px 1px 0 #2ab6f1, 1px -1px 0 #2ab6f1,
    -1px -1px 0 #2ab6f1;
}

</style>
