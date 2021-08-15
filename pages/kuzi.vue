<template>
  <v-container>
    <v-card class="pa-4">
      <p class="kekka_title">くじ引き</p>
      <div class="card_text">
        <p>くじを引こう</p>
      </div>
    </v-card>
    <div class="rand_area">
      結果は
      <div class="rand_name"></div>
      <button type="button" class="stop">ストップ！</button>
      <button type="button" class="restart" style="display: none">
        もう一度
      </button>
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
    var aryList = [
      '特賞',
      '1等',
      '２等',
      '３等',
      '４等',
      '５等',
      'はずれ',
      'はずれ',
    ]

    var key = 0
    var max_len = aryList.length - 1
    var randStart
    var speed = 25

    var randShuffle = function () {
      if (key > max_len) key = 0
      $('.rand_name').text(aryList[key])
      key++
    }

    randStart = setInterval(randShuffle, speed)
    $('.stop').click(function () {
      var random = Math.floor(Math.random() * (max_len + 1))
      $('.rand_name').text(aryList[random])
      clearInterval(randStart)
      $(this).hide()
      $('.restart').show()
      $('.present').show()
    })

    $('.restart').click(function () {
      $(this).hide()
      $('.present').hide()
      $('.stop').show()
      randStart = setInterval(randShuffle, speed)
    })
  })
}
</script>

<style>
.kekka_title {
  font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro',
    'Hiragino Mincho ProN', 'HGS明朝E', 'ＭＳ Ｐ明朝', serif;
  position: relative;
  padding: 1.5rem 2rem;
  -webkit-box-shadow: 0 2px 14px rgba(0, 0, 0, 0.1);
  box-shadow: 0 2px 14px rgba(0, 0, 0, 0.1);
  font-size: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 1px 1px 0 #000, -1px 1px 0 #000, 1px -1px 0 #000,
    -1px -1px 0 #000;
}
.kekka_title:before,
.kekka_title:after {
  position: absolute;
  left: 0;
  width: 100%;
  height: 4px;
  content: '';
  background-image: -webkit-linear-gradient(
    315deg,
    #704308 0%,
    #ffce08 40%,
    #e1ce08 60%,
    #704308 100%
  );
  background-image: linear-gradient(
    135deg,
    #704308 0%,
    #ffce08 40%,
    #e1ce08 60%,
    #704308 100%
  );
}

.kekka_title:before {
  top: 0;
}

.kekka_title:after {
  bottom: 0;
}
.card_text {
  font-size: 16px;
  display: flex;
  justify-content: center;
  align-items: center;
  padding-top: 1%;
  font-size: 2rem;
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

.stop {
  background-color: #e1ce08;
}

.restart {
  background-color: coral;
}
</style>
