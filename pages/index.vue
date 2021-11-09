<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole" style="position:relative">
      <img src="~assets/icon.png" alt="・" style="height:40px;margin-bottom:1em">
      <h1 style="display: inline-block;">文準通信/技術講座HOME</h1>
      <h2><nuxt-link to="/report/">文準通信（リンク）</nuxt-link></h2>
      <hr size=10 color="black" class="hrLine">
      <p><nuxt-link to="/report/">文準通信</nuxt-link>は一つのページにまとめます</p>

      <h2 id="hp">HP講座</h2>
      <hr size=10 color="black" class="hrLine">
      <ol>
        <li><nuxt-link to="/hp/kouhou/course1/">htmlの書き方基礎編（第一回HP講座）</nuxt-link>...htmlの書き方の基礎</li>
      </ol>
      
      <h2 id="movie">動画講座</h2>
      <hr size=10 color="black" class="hrLine">
      <ol>
        <li><nuxt-link to="/movie/course1/">動画編集のススメ（第一回動画講座）</nuxt-link>...動画編集のススメ/おすすめのソフト・インストール方法</li>
      </ol>

      <h2 id="other">その他</h2>
      <hr size=10 color="black" class="hrLine">
      <ol>
        <li><a href="/other/Illustrator.pdf">Illustrator講座完全版[PDF]</a>...AdobeIllustratorの完全版講座</li>
      </ol>
      <div style="height:200px"></div>
      <div style="width:100%;margin:0;background-color:#ee8888;text-align:center"><a href="https://forms.gle/oN1f6ecxgWkWeWPW7" style="color:black"><p style="font-size:1.5em">文化祭意見 BOXはこちら</p></a></div>
      <div style="width:100%;margin:0;background-color:#88ff88;text-align:center"><p style="font-size:1.5em">先行参団説明会：12/23</p></div>
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