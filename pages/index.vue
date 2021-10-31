<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole" style="position:relative">
      <img src="~assets/icon.png" alt="・" style="height:40px;margin-bottom:1em">
      <h1 style="display: inline-block;">文準通信/技術講座HOME</h1>
      <h2><nuxt-link to="/report">〇各文準通信（リンク）</nuxt-link></h2>
      <h2 id="hp">〇HP講座</h2>
      <ol>
        <li><nuxt-link to="/hp/kouhou/course1">htmlの書き方基礎編（第一回HP講座）</nuxt-link>...htmlの書き方の基礎</li>
      </ol>
      <h2 id="movie">〇動画講座</h2>
      <ol>
        <li><nuxt-link to="/movie/course1">動画編集のススメ（第一回動画講座）</nuxt-link>...動画編集のススメ/おすすめのソフト・インストール方法</li>
      </ol>
      <h2 id="other">〇その他</h2>
      <ol>
        <li><a href="/other/Illustrator.pdf">Illustrator講座完全版[PDF]</a>...AdobeIllustratorの完全版講座</li>
      </ol>
      <div style="height:500px"></div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
h2{
  font-size:20px
}
li{
  font-size:15px;
}
</style>