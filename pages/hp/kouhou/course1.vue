<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole">
      <course-title title="HP講座第一回" subtitle="htmlの書き方基礎編" date="2021/10/31" />
      <div class="containar" style="margin:0 5%;border:2px solid black;color:black">
        <div style="text-align:center;width:100%;"><p>▼目次▼</p></div>
        <ul class="row">  
          <nuxt-link v-for="(item,index) in items" v-bind:key="item.id" :to="'#'+index" class="col-md-6"><li>{{ item }}</li></nuxt-link> 
        </ul>
      </div>
      <article>
        <h2 id="0">はじめに</h2>
        <hr size=10 color="black" class="hrLine">
        <p style="text-indent:1em">これは来年の文化祭でオンライン文化祭（参団/広報係)に関わりたいと思っている方に向けたHP講座です。今年からは参団側でもコードを書いてもらう予定です。<!--そして、コードを書く予定がない人も<nuxt-link to="/hp/kouhou/yotei/">HPの進め方</nuxt-link>を一度見ていただけると嬉しいです。また、-->HP講座の今後の予定については<nuxt-link to="/hp/kouhou/housin/">HPの方針</nuxt-link>にまとめました。HPはオンライン文化祭の中心的な存在です。みんなで151st開成祭を盛り上げるていきましょう！</p>
        <p style="text-indent:1em">この講座ではHP作成の主にプログラミング部分をやったことのない・少ししか触ってない人のために0から教えていきます。（筆者は今年に入ってから始めて授業以外でhtmlを書き始めた未熟者なので温かい目で見てほしいです。ミスがあったらごめんなさい。）こんなのやったことあるぞ！という人はまぁ読む必要はありません。<!-- 作る側に回ってくれ！（<nuxt-link to="/hp/kouhou/boshu/">HP講座募集について</nuxt-link>）--></p>
      </article>
      <article>
        <h2 id="1">htmlとは？</h2>
        <hr size=10 color="black" class="hrLine">
        <p>ホームページを作るものです。Chromeとかブラウザで動かせます。ダブルクリックでだいたい動きます。</p>
      </article>
      <article>
        <h2 id="2">VisualStudioCodeの利用</h2>
        <hr size=10 color="black" class="hrLine">
        <article>
          <h3>1.インストール</h3>
          <p>VisualStudioCodeとはhtml等、プログラムを書きやすくするためのアプリです。"VSCode"と呼ばれることも多いです。（VisualStudioは別のアプリ）</p>
          <ol class="clearnum">
            <li>① 次のリンクにアクセスします：<a href="https://code.visualstudio.com/Download">https://code.visualstudio.com/Download</a></li>
            <li>② 自分の使っているOSに合わせて ↓Windows または ↓Mac を押してダウンロードします（※わからない人はPC本体にリンゴのマークがあればMac、そうでなければだいたいWindowsです）</li>
            <li>③ インストーラーを立ち上げます。</li>
            <li>④ インストールボタンを押し、後は流れに沿って進んでください。</li>
          </ol>
          <p>以上でインストールは完了です。</p>
          <p>（補足）</p>
          <ul>
            <li>デフォルトの言語設定は英語となっていますが、日本語に直すこともできます。（詳しくは<a href="https://www.javadrive.jp/vscode/install/index4.html">https://www.javadrive.jp/vscode/install/index4.html</a>を参照してください。）</li>
            <li>文字数が多くても画面の端で折り返すようにすようにすることができます。（詳しくは<a href="https://www.javadrive.jp/vscode/setting/index7.html">https://www.javadrive.jp/vscode/setting/index7.html</a>参照してください。）</li>
          </ul>
        </article>
        <article>
          <h3 id="makefile">2.htmlファイル作成</h3>
          <ol class="clearnum">
            <li>① 左上の ファイル(F) から 新規ファイル を押します。</li>
            <li>② Untitled-1 というものが出てきます。</li>
            <img src="htmlmake.png" alt="ファイル作成" style="width:60%;margin:10px 20%">
            <li>③ 左上の ファイル(F) から 名前を付けて保存 を押します。</li>
            <li>④ 保存したい場所に移動させます。</li>
            <li>⑤ ○○.htmlという名前で保存します。（例：あいうえお.html）</li>
            <img src="htmlsave.png" alt="htmlとして保存" style="width:60%;margin:10px 20%">
          </ol>
          <p>以上でhtmlファイルの作成が完了です。次に進んでください。</p>
        </article>
      </article>
      <article>
        <h2 id="3">書き始め</h2>
        <hr size=10 color="black" class="hrLine">
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
  &lt;/head>
  &lt;body>
    &lt;!-- この下から書き始める -->

  &lt;/body>
&lt;/html></pre>
        <p>丸々コピーして貼り付けてください。&lt;!-- この下から書き始める -->の次の行から書き始めます。</p>
      </article>
      <article>
        <h2 id="4">htmlの書き方</h2>
        <hr size=10 color="black" class="hrLine">
        <p>&lt;h1>と&lt;/h1>、&lt;p>と&lt;/p>など"タグ"で文字を囲います。</p>
        <p>・記述例（h1やdivなどについては<nuxt-link to="#5">次の章</nuxt-link>、style=""については<nuxt-link to="#7">スタイルの章</nuxt-link>で説明します）</p>
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
  &lt;/head>
  &lt;body>
    &lt;!-- この下から書き始める --><font color="red">
    &lt;h1>151st開成祭&lt;/h1>
    &lt;h2>151は"st"&lt;/h2>
    &lt;p>150thに慣れすぎていると151thと言ってしまいそうになることもあるが151は"st"である&lt;/p>
    &lt;a href="https://151st-kaiseifes-bunjun.vercel.app/hp/kouhou/course1">HP講座のリンク&lt;/a>
    &lt;p>他の年&lt;/p>
    &lt;div style="padding:20px;background-color:#eeeeee">
      &lt;p>152→152&lt;span style="font-weight:bold">nd&lt;/span>&lt;/p>
      &lt;p>153→153rd&lt;/p>
      &lt;p>154~9→15〇th&lt;/p>
    &lt;/div>
    &lt;p>151thという言い方がないわけではないらしい&lt;/p>
    &lt;img src="images/picture.png" alt="写真の写真">&lt;/img></font>
  &lt;/body>
&lt;/html></pre>
        <p>・実行結果（エクスプローラー等で作ったファイルをダブルクリックしてください）※写真を入れていないので&lt;img>の部分がうまく表示されません。imgタグの使い方や実行結果は調べてやってみてください。</p>
        <div class="reset" style="border:1px solid black;margin:5px;width:100%;padding:5px">
          <h1>151st開成祭</h1>
          <h2>151は"st"</h2>
          <p>150thに慣れすぎていると151thと言ってしまいそうになることもあるが151は"st"である</p>
          <a href="https://151st-kaiseifes-bunjun.vercel.app/hp/kouhou/course1">HP講座のリンク</a>
          <p>他の年</p>
          <div style="padding:20px;background-color:#eeeeee">
            <p>152→152<span style="font-weight:bold">nd</span></p>
            <p>153→153rd</p>
            <p>154~9→15〇th</p>
          </div>
          <p>151thという言い方がないわけではないらしい※諸説あり</p>
          <img src="images/picture.png" alt="写真の写真"><img>
        </div>
        <h3>説明</h3>
        <p style="text-indent:1em">「&lt;h1>151st開成祭&lt;/h1>」で見出し(=h1)の文字を151st開成祭(=&lt;h1>&lt;/h1>で囲まれた部分)にするという意味です。見出しならh1、段落ならpといったのは次の章で紹介します。使っていくうちになれると思います。</p>
        <p>（重要な補足）<br>　「　」（全角スペース）は使わないように気を付けましょう。よくこれが原因でエラーになります。&lt;p>&lt;/p>などに挟まれたところ以外で全角は使わないようにしてください。</p>
        <p>（補足）<br>　どこがエラーなのか分からないといったときにはブラウザで開いてからWindowsの場合はF12、Macの場合は⌘+option+iを押して<u>デベロッパーツール</u>を開いてください。（ものによって違うかもしれません。上手くいかなかったら使っているブラウザ・OSを入れて検索してみてください）ブラウザによって違いますが赤いものがあったらエラーの可能性が高いです。そしてそこの()内にファイルと行数が指定されていることが多いのでそこをまず見てみてください。分からなかった場合は一般的な言葉にして検索して下さい。また、たまに再度読み込みをすると上手くいく場合もあるのでそちらも一回試してみてください。</p>
      </article>
      <article>
        <h2 id="5">よく使うタグ</h2>
        <hr size=10 color="black" class="hrLine">
        <ul>
          <li>&lt;h1>,&lt;h2>,&lt;h3>...など<br>見出し。上の記述例のように文字を入れる。文字が大きい。</li>
          <li>&lt;p><br>普通の段落。同様に上の記述例のように文字を入れる。</li>
          <li>&lt;a><br>リンク付きの文字。href=""の中にクリックして飛ぶ先のリンクを書く。文字が青くなる。&lt;p>と&lt;/p>の間に入れる</li>
          <li>&lt;div><br>他のタグを囲むもの。改行する。</li>
          <li>&lt;span><br>他のタグを囲むもの。改行しない。</li>
          <li>&lt;img><br>画像の表示。srcには画像のリンク（相対パス等を検索）、altには画像の説明を入れる。「html img」で検索するとよい。</li>
        </ul>
        <p style="text-indent:1em">他にもタグはあります。「html 下線」のように検索すれば&lt;u>、「html 箇条書き」のように検索すれば&lt;li>みたいに色々出てくると思います。数も多いですし自分で検索してみましょう！</p>
      </article>
      <article>
        <h2 id="6">演習問題（よく使うタグ）</h2>
        <hr size=10 color="black" class="hrLine">
        <p>以下のものを再現してみよう！</p>
        <div class="reset" style="border:1px solid black;margin:5px;width:100%;padding:5px">
          <h1>改行について（タイトル）</h1>
          <h2>brタグについて（サブタイトル）</h2>
          <p>brタグはかなり簡単に改行することができます。しかしデザインを整えるために使うのは避けましょう。（本文）</p>
          <p>詳細は<a href="https://style.potepan.com/articles/20710.html">こちら</a>（https://style.potepan.com/articles/20710.html）</p>
        </div>
        <p>解答は<nuxt-link to="#10">下の方</nuxt-link>にあります</p>
      </article>
      <article>
        <h2 id="7">スタイル</h2>
        <hr size=10 color="black" class="hrLine">
        <p>背景の色を変えたり文字の大きさを変えたりしたい！といったときにはスタイルを設定します。</p>
        <p style="text-indent:1em">本来は他ページに使いまわしができる上に読みやすくなる為cssファイルを別に利用した方がいいのですがここでは「css埋め込み・style属性」で設定しようと思います。外部ファイルcssについては<a href="https://saruwakakun.com/html-css/reference/where-css">https://saruwakakun.com/html-css/reference/where-css</a>が参考になります。css埋め込み（styleタグの中身）をcssファイルにうつしてheadにlinkを書くことで外部ファイルcssにすることができます。</p>
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8"><font color="red">
    &lt;style>
      h1{
        font-size:10px;
      }
      .sousyoku{
        padding:2vw;
        border:1px solid black;
        background-color:#eeeeee;
      }
    &lt;/style></font>
  &lt;/head>
  &lt;body>
    &lt;!-- この下から書き始める --><font color="blue">
    &lt;h1>小さな文字に変化したタイトル&lt;/h1>
    &lt;div <font color="red">class="sousyoku"</font>>
      &lt;p>普通の文字&lt;/p>
      &lt;p <font color="red">style="color:red"</font>>赤文字&lt;/p>
    &lt;/div></font>
  &lt;/body>
&lt;/html></pre>
        <p>・実行結果※疑似的な物になっています</p>
        <div class="reset" style="border:1px solid black;margin:5px;width:100%;padding:5px">
          <h1 style="font-size:10px">小さな文字に変化したタイトル</h1>
          <div class="sousyoku">
            <p>普通の文字</p>
            <p style="color:red">赤文字</p>
          </div>
        </div>
        <p style="text-indent:1em">font-size:10pxとは文字の大きさを10pxに、color:redは文字の色を赤色にするという意味です。スタイルは数が多いので説明しきれません。例えば影をつけたいと思ったら「html 影」と検索すればbox-shadowなどと出てきます。種類が多いので調べるようにしましょう。</p>
        <h3>説明</h3>
        <p style="text-indent:1em">&lt;style>&lt;/style>に囲まれた所とclass=""となっている所がcss埋め込みです。そしてstyle=""の部分がstyle属性です。</p>
        <ul class="ulstyle">
          <li>css埋め込み（h1の部分）<br>このようにタグの名前をそのまま書くとそのhtmlファイル内の全てのh1（書いたタグ）にstyleが適用されます。</li>
          <li>css埋め込み（「.sousyoku」の部分）<br>このように「.○○」といったようにするとclassを作ることができます。class="○○"という属性がついた要素にstyleが適用されます。</li>
          <li>style属性の部分<br>style=""という属性をつけることによってその要素にstyleを適用できます。</li>
        </ul>
        <p>つまり、使い分けとしては</p>
        <ul class="ulstyle">
          <li>タグ名(h1のやつ)<br>ページ丸ごと変えるので全てに適用したいお気に入りのスタイルを書きます</li>
          <li>class(.○○のやつ)<br>複数箇所で同じスタイルを使う場合に利用します。複数人でページを作るときはこれでやることが推奨されます。また、一か所でしか使わなくても設定するスタイルの数が多ければclassを利用した方がコードが読みやすくなるので良いです。</li>
          <li>style属性の部分<br>一個だけ使うとき・classを設定するよりそのまま書いた方が量が減る時に使います。複数箇所で使うならclassの方がコードを読みやすいのでclassを利用してください。</li>
        </ul>
        <p>といった感じになります。</p>
        <p>（補足）<br>　class="sousyoku tyousyoku"のようにスペースを開けると二つのclassを設定できます。また、style="color:red;background-color:green;"のように「;」で挟むことでstyle属性に複数のスタイルを設定できます。</p>
        <p>以上で今回のスタイルについての説明は終了です。</p>
      </article>
      <article>
        <h2 id="8">あとがき</h2>
        <hr size=10 color="black" class="hrLine">
        <p style="text-indent:1em">まず、ここまで読んでいただきありがとうございます。そして、ここまでお疲れさまでした。第一回なのに量が多かったと思います。そして、HP作成は経験量が大事です。新たなタグやスタイルを使う場面ができたり、自分のお気に入りのデザインを見つけることができたりします。是非作ってみてください！（作ってもらう企画も考えています）<!--もう少しやりたい！という方は是非、<nuxt-link to="/hp/kouhou/boshu">講座募集</nuxt-link>に出していただけると嬉しいです。-->それではまた次回以降もよろしくお願いします。次回はhtmlの難しい部分、padding/marginやdisplayなどをやる予定です。</p>
      </article>
      <article>
        <h2 id="9">この講座のデザインについて</h2>
        <hr size=10 color="black" class="hrLine">
        <p>参考までに</p>
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
    &lt;style>
      h2{
        font-size:25px;
        margin-top:25px;
      }
      h3{
        font-size: 20px;
      }
      .back{
        margin:auto;
        padding:40px;
        background-color:white;
        box-shadow:0px 0px 5px 1px rgb(200, 200, 200);
        max-width:800px;
      }
    &lt;/style>
  &lt;/head>
  &lt;body style="margin:0;">
    &lt;div style="background-color:rgb(220,220,220);">
      &lt;div class="back">
        &lt;!-- この下から文章を書く -->
        &lt;h1>講座１&lt;/h1>
        &lt;h2>「&amp;lt;>」の書き方&lt;/h2>
        &lt;div style="padding:2vw;background-color:#eeeeee;">
          &lt;p>普通に書くとコードとして扱われてしまうため、&amp;amp;lt;と書くことで&amp;lt;と表示できる（>はそのままで問題ない）&lt;/p>
        &lt;/div>
        &lt;div style="border:1px solid black;margin:5px;width:100%;padding:5px">
          &lt;p>「&amp;amp;lt;」を利用してコードを表示しよう！&lt;/p>
        &lt;/div>

      &lt;/div>
    &lt;/div>
  &lt;/body>
&lt;/html></pre>
      </article>
      <article>
        <h2 id="10">※解答</h2>
        <hr size=10 color="black" class="hrLine">
        <p><nuxt-link to="#6">この問題</nuxt-link>の解答例です</p>
        <pre style="padding:2vw;background-color:#eeeeee">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
  &lt;/head>
  &lt;body>
    &lt;!-- この下から書き始める -->
    &lt;h1>改行について（タイトル）&lt;/h1>
    &lt;h2>brタグ（サブタイトル）&lt;/h2>
    &lt;p>brタグはかなり簡単に改行することができます。（本文）&lt;/p>
    &lt;p>詳細は&lt;a href="https://style.potepan.com/articles/20710.html">こちら&lt;/a>（https://style.potepan.com/articles/20710.html）&lt;/p>
  &lt;/body>
&lt;/html></pre>
          <p style="text-indent:1em;">最後から三行目の&lt;a>&lt;/a>を改行することもできますが文章のまとまりが分かりにくくなる為、筆者は同じ行に書いています。どちらでも同じです。</p>
      </article>
    </div>
  </div>
</template>

<style scoped>
.ulstyle li {
  margin-bottom: 10px;
}
.reset h2{
  font-size:2rem;
  margin-top:0;
  margin-bottom: 0.5rem;
}

.sousyoku{
  padding:2vw;
  border:1px solid black;
  background-color:#eeeeee;
}
</style>
<script>
import { defineComponent } from '@vue/composition-api'

export default {
  data (){
    return{
      items:["はじめに","htmlとは？","VisualStudioCodeの利用","書き始め","htmlの書き方","よく使うタグ","演習問題（よく使うタグ）","スタイル","あとがき","この講座のデザインについて","演習問題の解答"]
    }
  },
}
</script>
