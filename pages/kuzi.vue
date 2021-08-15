<template>
  <v-container>
    <v-card class="pa-4">
      <p class="kekka_title">くじ引き</p>
      <div class="card_text">
        <p>くじを引こう</p>
      </div>
    </v-card>
    <div class="rand_area">
    あなたの運勢は
      <div class="rand_name"></div>
      <button type="button" class="stop">ストップ！</button>
      <button type="button" class="restart" style="display: none">
        もう一度
      </button>
      <div class="present_item"></div>
      <button type="button" class="present" style="display: none">プレゼントを受け取る</button>
    </div>
  </v-container>
</template>
<script>
export default {
  head() {
    return {
      script: [
        {
          src: 'https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js',
        },
      ],
    }
  },
}
if (process.client) {
  $(function () {
    //候補を配列で設定
    var aryList = ['特賞', '1等', '２等', '３等', '４等', '５等', 'はずれ','はずれ']
    var presentList=['n','a','a','a','a','a']
    //グローバル変数
    var key = 0
    var max_len = aryList.length - 1
    var randStart
    var speed = 20 //シャッフルスピード

    //文字シャッフル関数
    //20ミリ秒毎に候補の文字列をシャッフルさせる
    var randShuffle = function () {
      if (key > max_len) key = 0
      $('.rand_name').text(aryList[key])
      key++
    }
    //文字シャッフル開始
    randStart = setInterval(randShuffle, speed)

    //回転を止める（抽選結果）
    $('.stop').click(function () {
      var random = Math.floor(Math.random() * (max_len + 1)) //ランダムで配列の数を取得
      $('.rand_name').text(aryList[random]) //対象の数値に該当する文字を表示
      clearInterval(randStart) //シャッフルストップ
      $(this).hide() //止めるボタンの非表示
      $('.restart').show() //再開ボタンの表示
      $('.present').show()
    })

    //回転を再開する
    $('.restart').click(function () {
      $(this).hide() //再開ボタンの非表示
      $('.present').hide()
      $('.stop').show() //止めるボタンの表示
      randStart = setInterval(randShuffle, speed) //シャッフル再開
    })
    $('.present').click(function () {
      $('.present_item').text(presentList[random]) 
      $(this).hide()
      $('.restart').hide() //再開ボタンの非表示
      $('.present').hide()
      
    })
  })
}
</script>

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
.rand_area {
  box-sizing: border-box;
  border: 2px solid #ccc;
  padding: 10px 10px 20px 10px;
  text-align: center;
}

.rand_name {
  font-weight: bold;
  font-size: 30px;
  text-align: center;
}

.rand_area button {
  border-radius: 5px;
  font-weight: bold;
  font-size: 18px;
  padding: 5px 15px;
  color: #fff;
  margin-top: 10px;
  cursor: pointer;
}
.present_item{
  font-weight: bold;
  font-size: 30px;
  text-align: center;
}


.stop {
  background-color:#e1ce08;
}

.restart {
  background-color:coral;
}
.present{
    background-color: crimson;
}
</style>
