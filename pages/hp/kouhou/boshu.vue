<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole indent">
      <course-title title="HP講座募集" subtitle="HP講座募集について" date="2021/11/12"/>
      <course-contents :items="items" />
      <section>
        <h2 id="0">はじめに</h2>
        <hr size="10" color="black" class="hrLine">
        <p>HPの講座を募集します。たぶん僕より上手く書ける人も多いと思います。みんな書いてくれ！！！（文責：4745/SC）</p>
      </section>
      <section>
        <h2 id="1">形式</h2>
        <hr size="10" color="black" class="hrLine">
        <h3>html</h3>
        <p>Googleドライブやメールで送ってください。Nuxt.js化して上げます。写真とかも忘れずにつけてください（動画の場合はYouTube埋込みを使います。動画と埋込みコードリンク抜きをコード内に入れてください）</p>
        <h3>Nuxt.js</h3>
        <p>GoogleドライブでもGitHubでもOKです。写真等は上と同じです。</p>
        <h3>PDFなどその他形式</h3>
        <p>HPの講座作成はHPを書く経験も兼ねているのでこの形式ではなく上の2つのどちらかでお願いします。</p>
      </section>
      <section>
        <h2 id="2">内容</h2>
        <hr size=10 color="black" class="hrLine">
        <p>〇〇苦労したとか〇〇かっこよくない？とかそんな感じで大丈夫です。（例：リンク）もちろん完全版でもありがたいです。</p>
        <h3>分類（※10月31日現在）</h3>
        <p>HTML/GitHub/Nuxt.js(＆boostrap)/Django/デザイン/Figma/SEO/その他</p>
        <h3>特に募集中の記事</h3>
        <p style="text-indent:0">書くことが思いつかないという人は是非この下の話題を選んでみてください</p>
        <ol>
          <li>HTMLのheadの中に書くもの</li>
          <li>GitHubの理論（とか色々！）</li>
          <li>Django（第6回書きたい人は連絡お願いします）</li>
          <li>Figma</li>
          <li>SEO対策</li>
          <li>おすすめのデザイン（classも入れて）</li>
        </ol>
        <p style="text-indent:0">その他、思いついたことがあったら連絡お願いします。</p>
      </section>
      <section>
        <h2 id="3" style="color:red">注意事項</h2>
        <hr size=10 color="black" class="hrLine">
        <p>基本、このホームページに掲載します。しかし、文化祭全体のHPにも載せる可能性があります。また、来年以降も使う可能性があります。また、<u style="color:red">ネット上に公開している</u>ので名前や個人が特定できる写真を掲載する場合は<u style="color:red">保護者の許可を取るよう</u>にお願いします。（僕は面倒事になるのは嫌なので載せてません）そして不適切な内容を入れるのはやめてください。投稿するものは僕が確認した上で、顧問の先生にも確認していただくことになるので注意してください。また、当然著作権には違反しないよう注意してください。</p>
      </section>
      <section>
        <h2 id="4">送り先</h2>
        <hr size=10 color="black" class="hrLine">
        <p style="text-indent:0;">メールかDiscordにあげるということ・そして場合によっては本体を添付してください。GitHubのみにするのはやめてください。注意事項を確認するためです。</p>
        <ol class="clearnum" style="overflow:hidden">
          <li>メールアドレス：151stksfeshpmanage@gmail.com</li>
          <li>Discord：tsym_4745#1731（広報SC山下のアカウント）</li>
          <li>GitHub：<a href="https://github.com/tsym77yoshi/151st_kaiseifes_bunjun">https://github.com/tsym77yoshi/151st_kaiseifes_bunjun</a>（追加先はhpの各分類の下、kouhou外）</li>
        </ol>
        <p style="text-indent:0;">※返信遅くなったらすみません</p>
      </section>
      <section>
        <h2 id="5">例</h2>
        <hr size=10 color="black" class="hrLine">
        <section>
          <h3>htmlの場合(例)</h3>
          <p style="text-indent:0">メール</p>
          <pre style="padding:2vw;background-color:#f9f9f9;border:1px solid black">
・差出人：&lt;!-- @kaiseigakuen.jpで（本人確認をしたい） -->
・宛先：151stksfeshpmanage@gmail.com
・件名：HP講座

・本文：

分類：おすすめのデザイン
タイトル：HPに動きをつけよう！
サブタイトル：hoverについて
日付：2021/11/12

html：
&lt;!-- 省略・ここにコピペでもGoogleDriveでもなんでもよい -->
テンプレート１=><nuxt-link to="#example">下の方</nuxt-link>

画像：
&lt;!-- 省略・欠かさないよう注意・どこで使っているかも明記 -->

動画：
&lt;!-- どうにかして送ってください・YouTube限定公開を使うつもりでいます -->

※もし名前を載せる場合
保護者から許可を　とりました or とってません（とっていない場合は名前を消してから送ってください）
          </pre>
        </section>
        <section>
          <h3>Nuxt.jsの場合</h3>
          <p style="text-indent:0;">※メールも送ってください。気づけない＆確認を取りたいからです</p>
          <ul>
            <li>GitHub：<a href="https://github.com/tsym77yoshi/151st_kaiseifes_bunjun">https://github.com/tsym77yoshi/151st_kaiseifes_bunjun</a></li>
            <li>メール：151stksfeshpmanage@gmail.com（上のhtmlを参考にしてください）</li>
            <li>Discord：tsym_4745#1731（広報SC山下のアカウント）</li>
          </ul>
          <p style="text-indent:0">pagesフォルダの中のhpフォルダの中のtemplate.vueです。参考までに（使わなくても勿論問題ないです）：<nuxt-link to="/hp/template1">テンプレート１のページ</nuxt-link></p>
        </section>
      </section>
      <section>
        <h2 id="6">その他</h2>
        <hr size=10 color="black" class="hrLine">
        <p>何か質問とか修正とかがあればdiscordかメールにお願いします。GitHubでの連絡方法は分かりません⊂( *･ω･ )⊃。HP担当の4桁番号：4745　4846</p>
        <p>これはある意味練習なのでここで失敗していってください。ジャンジャン送ってきて！！（僕らも失敗します。そこは温かい目で見ていただけると嬉しいです）</p>
      </section>
      <section>
        <h2 id="example">htmlのテンプレート</h2>
        <hr size=10 color="black" class="hrLine">
        <h3>course.html</h3>
        <p style="text-indent:0">外部css化はhtml上では絶対ですがNuxt.js的にはファイルが増えるので少し微妙です。埋め込みの方がいいです。</p>
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
    &lt;link rel="stylesheet" href="default.css">
    &lt;style>

    &lt;/style>
  &lt;/head>
  &lt;body style="margin:0;">
    &lt;!-- ヘッダー自動追加 -->
    &lt;div style="background-color:rgb(220,220,220);">
      &lt;div class="whole">
        &lt;!-- タイトルはメールの内容を反映します（Vue.jsのコンポーネントを利用しているため）
          別のものを自分でつけたい場合はつけてください -->
        &lt;!-- 目次も同様です（Vue.jsのコンポーネントを利用しているため）
          別のものを自分でつけたい場合はつけてください -->
        
        &lt;section>
          &lt;!-- idは目次で利用しています -->

          &lt;h2 id="0">はじめに&lt;/h2>
          &lt;hr size="1" color="black" class="hrLine">

          &lt;p style="text-indent:1em">４桁番号が書いてあると質問しやすいかもしれません&lt;/p>
        &lt;/section>
        &lt;section>
          &lt;h2 id="1">第2章&lt;/h2>
          &lt;hr size="1" color="black" class="hrLine">
          &lt;p style="text-indent:1em">texttexttext&lt;/p>
        &lt;/section>
        &lt;section>
          &lt;h2 id="2">「&amp;lt;」の書き方&lt;/h2>
          &lt;hr size="1" color="black" class="hrLine">
          &lt;div style="padding:2vw;background-color:#eeeeee;">
            &lt;p>普通に書くとコードとして扱われてしまうため、「&amp;amp;lt;」と書くことで「&amp;lt;」と表示できる（「>」はそのままで問題ない）&lt;/p>
          &lt;/div>
          &lt;div style="border:1px solid black;margin:5px;width:100%;padding:5px">
            &lt;p>「&amp;amp;lt;」を利用してコードを表示しよう！&lt;/p>
          &lt;/div>
        &lt;/section>

        &lt;!-- 分類のリンクはメールの内容を反映します（Vue.jsのコンポーネントを利用しているため）
          別のものを自分でつけたい場合はつけてください -->

      &lt;/div>
    &lt;/div>
    &lt;!-- フッター自動追加 -->
  &lt;/body>
&lt;/html></pre>
<h3>default.css</h3>
<p style="text-indent:0">css（コピペするのみで送らなくて大丈夫です。ここには自分で追記せずに、追記する場合は埋め込みでお願いします。）</p>
<pre style="padding:2vw;background-color:#eeeeee">
.whole{
  /*全体につける。index.vueで例を見るのが良いと思う*/
  margin:auto;
  padding:40px;
  background-color:white;
  box-shadow:0px 0px 5px 1px rgb(200, 200, 200);
  max-width:800px;
}
.whole h2{
  font-size:25px;
  margin-top:25px;
}
.whole h3{
  font-size: 20px;
  margin-top: 20px;
}
.whole section{
  margin-bottom: 3em;
}
@media screen and (max-width: 639px) {
  .whole{
    padding:40px 0.5em;
  }
}

.indent p{
  /*インデントをしたい記事の親要素につける*/
  text-indent: 1em;
}
.clearnum li{
  /*数字を消したいliの親要素のul/ol要素につける*/
  list-style: none;
  text-indent: -1.3em;
}
.hrLine{
  /*水平ライン(h2の下)*/
  width:102%;
  margin:0 -1% 1em;
}

body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.5;
    color: #212529;
    text-align: left;
    background-color: #fff;
}
html {
    font-family: sans-serif;
    line-height: 1.15;
    -webkit-text-size-adjust: 100%;
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
h1, h2, h3, h4, h5, h6, .h1, .h2, .h3, .h4, .h5, .h6 {
    margin-bottom: 0.5rem;
    font-weight: 500;
    line-height: 1.2;
}</pre>
      </section>
      <course-link-index type1="HP講座" type1link="/hp/index/" type2="by広報総務" type2link="/#hp" />
    </div>
  </div>
</template>

<style scoped>
.ulstyle li {
  margin-bottom: 10px;
}
</style>

<script>
export default {
  data (){
    return{
      items:["はじめに","形式","内容","注意事項","送り先","例","その他"]
    }
  },
}
</script>