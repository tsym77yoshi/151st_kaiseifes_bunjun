<template>
    <div style="background-color:rgb(220,220,220);">
        <div class="whole">
            <course-title title="HP講座第二回" subtitle="htmlの書き方基礎編" date="2021/10/31" />
            <div class="containar" style="margin:0 5%;border:2px solid black;color:black">
              <div style="text-align:center;width:100%;"><p>▼目次▼</p></div>
              <ul class="row">  
                <nuxt-link v-for="(item,index) in items" v-bind:key="item.id" :to="'#'+index" class="col-md-6"><li>{{ item }}</li></nuxt-link> 
              </ul>
            </div>
            
            <article>
            <h2 id="0">はじめに</h2>
            <hr size=10 color="black" class="hrLine">
            <p style="text-indent: 1em;">これは来年の文化祭でオンライン文化祭（参団/広報係)に関わりたいと思っている方に向けたHP講座の第二回です。
            第一回では環境の構築やhtmlの基礎的な書き方などを学びましたが第二回ではcssについても詳しく解説しつつ、ホームページを実際に作るための準備を進めていきます。
         <br>第一回とは筆者が違うので至らないところがあるかもしれませんがよろしくお願いします。</p>
            </article>

            <article>
                <h2 id="1">よく使うタグ(補足)</h2>
                <hr size=10 color="black" class="hrLine">
                <p>まずは第一回　よく使うタグ の補足から入ります。<br>第一回では、aタグなど基本的なタグを紹介しましたがこれらのタグ全てが同じ書き方で書けるわけではありません。
                タグごとに指定できる属性が異なったりなどはもちろん、大きな違いとして終了タグ(一つの要素の最後につける&lt;/～>)があるか否かという違いが挙げられます。以下によく使うタグを終了タグのありなしによって分類しましたので復習がてら確認してみてください。</p>
                <h3>終了タグがあるタグ</h3>
                <ul class="ari">
                    <li>&lt;h1>,&lt;h2>,&lt;h3>...など<br>見出し。第一回の記述例のように文字を入れる。数字が小さいほど文字が大きい。</li>
                    <li>&lt;p><br>普通の段落。同様に第一回の記述例のように文字を入れる。</li>
                    <li>&lt;a><br>リンク付きの文字。href=""の中にクリックして飛ぶ先のリンクを書く。文字が青くなる。&lt;p>と&lt;/p>の間に入れる</li>
                    <li>&lt;div><br>他のタグを囲むもの。改行する。基本的にどんな要素でも入るので濫用しがち。</li>
                    <li>&lt;span><br>他のタグを囲むもの。改行しない。inline要素(下で解説)しか入りません。</li>
                    <li>&lt;ul>,&lt;ol>,&lt;li><br>箇条書きするのに使います。</li>
                </ul>
                <h3>終了タグがないタグ</h3>
                <ul class="nasi">
                    <li>&lt;img><br>画像の表示。srcには画像のリンク（相対パス等を検索）、altには画像の説明を入れる。「html img」で検索するとよい。</li>
                    <li>&lt;br><br>pタグなどの中に入れるとその地点で必ず改行される。</li>
                    <li>&lt;hr><br>線を引くタグ。見出しに下線をつける時などに使う。</li>
                    <li>&lt;input><br>入力欄やボタンなどユーザーからの情報を受け取るときに使います。</li>
                </ul>
                <p>第一回でも述べましたが他にもタグはたくさんあるのでどんなタグを使えばいいのか、それはどう書けばよいのかが分からなくなったらすぐ調べるのが良いです。</p>
            </article>

            <article>
                <h2 id="2">cssの外部化</h2>
                <hr size=10 color="black" class="hrLine">
                <p>さて、この第二回ではcssについてそれなりに詳しくやる予定なのですがそれにあたり予めやっておくべきことが一つあります。
                    それがcssの外部化です。第一回のコードの記述例ではcssはstyle=""を使いhtmlファイル内で要素の色、余白などを調整していましたが.cssを拡張子に持つテキストファイルを別に用意することで
                    htmlファイルはサイトの内容、cssファイルはサイトの装飾というように役割が分かれ分かりやすいコードを書くことが出来ます。簡単にできるのでさっさとやってしまいましょう。
                </p>
                <ol>
                    <li>① .cssを拡張子に持つテキストファイルをhtmlファイルと同じ場所に作ります。</li>
                    <li>② htmlファイルのheadタグの中に&lt;link rel="stylesheet" href="cssのファイル名">を書きます。ちなみにこのlinkタグも終了タグはありません。</li>
                    <li>③ cssファイルにhtmlファイルの内容に従ってコードを書きます。</li>
                </ol>
                <p>これだけです。また、javascriptを使う場合もこれと同じような方法で外部化をすることができます。</p>
            </article>

            <article>
                <h2 id="3">cssとhtmlの対応</h2>
                <hr size=10 color="black" class="hrLine">
                <p style="text-indent: 1em;">cssを書く準備が出来たところでcssをhtmlと対応させる方法を紹介します。
                   <br>そこで重要なのがhtml内の要素にclassもしくはidを設定することです。classもidも例えばdiv要素にそれを設定する場合、
                   &lt;div class="好きな名前"> や &lt;div id="好きな名前"> という風に開始タグを書くことで設定することが出来ます。
                   classは同ページ内の複数の要素に同じclassを割り当てることが出来ますが、idでは同じidは別の要素には割り当てが出来ません。
                   なので基本的にはclass、特別なものに対してはidを割り当てるという認識で大丈夫です。<br>
                </p>
                <p style="text-indent: 1em;">
                    それでは指定したclassやidにcssを適用していきましょう。<br>
                    作ったcssファイルに .クラス名{} や #id名{} と書き、{}のなかにスタイルの指定を書いていくだけです。(良く使うスタイルは下で紹介しています)
                    またbodyやh1、pタグなど元からあるタグに関しては body{} という風に書くことでそのタグを使う要素すべてにcssの適用ができ、上の書き方と併用して、
                     .class名 p{} というように書けば特定のclassのp要素のみにcssが適用できます。<br>
                    そしてcssは基本的に小さいくくりに対して適用したものが優先されます。下の記述例を確認してください。
                </p>
                <p>test.html</p>
                <pre style="padding:2vw;background-color:#eeeeee;margin: 1vw;">
                    &lt;!DOCTYPE html>
                    &lt;html>
                      &lt;head>
                        &lt;meta charset="utf-8">
                        &lt;link rel="stylesheet" href="test.css">
                      &lt;/head>
                      &lt;body>
                        &lt;h1>これはh1要素です&lt;/h1>
                        &lt;div class="green">
                          &lt;h2>これはh2要素です&lt;/h1>
                          &lt;p>これはp要素です&lt;/p>
                        &lt;/div>
                      &lt;/body>
                    &lt;/html>
                </pre>
                <p>test.css</p>
                <pre style="padding:2vw;background-color:#eeeeee;margin: 1vw;">
                    body{color: black}
                    .green{color: green;}
                    .green p{color: red}                   
                </pre>
                <p>実行結果</p>
                <div class="reset" style="border:1px solid black;margin:5px;width:100%;padding:5px">
                    <h1 style="color: black;">これはh1要素です</h1>
                    <h2 style="color: green;">これはh2要素です</h2>
                    <p style="color: red;">これはp要素です</p>
                </div>
            </article>

            <article>
                <h2 id="4">良く使うスタイル</h2>
                <hr size=10 color="black" class="hrLine">
                <ul>
                    <li>color: ～;<br>文字の色を変えることが出来る。～に色の名前やRGBの値を入れることで指定する。</li>
                    <li>background: ～;<br>背景の色を変えることが出来る。～に色の名前やRGBの値を入れて指定する。</li>
                    <li>text-aline: ～;<br>～にcenterやrightを入れることで文字を中央ぞろえや右そろえにできる。<br>「その要素の中での」中央ぞろえや右そろえなので文字が要素の中いっぱいに詰まっている場合は何も変わらない。</li>
                    <li>padding、margin、borderなど<br>余白などを調節できる。とても重要なので下で個別に解説。</li>
                    <li>display: ～;<br>表示形式を変更できる。とても重要なので下で個別に解説。</li>
                    <li>overflow-x: ～;<br>x方向(横方向)で画面からはみ出る部分の処理を変えられる。～にhiddenを入れると横スクロールバーを消してくれるので便利。</li>
                </ul>
                <p>他にもたくさんのスタイルがあるのでhtmlのタグと同様に困ったら調べてみるのが良いでしょう。</p>
            </article>

            <article>
                <h2 id="5">padding、marginなどの関係性</h2>
                <hr size=10 color="black" class="hrLine">
                <p>上で良く使うスタイルを紹介しましたがその中で最も重要なのがpaddingやmarginです。これらの関係性を理解すればサイト内の余白を自由自在に調節することが出来ます。
                    ここで下の写真を見てください。余白の調整に使えるものの関係はそのようになっています。
                </p>
                <p><img src="box-model2.png" alt="図" style="width:60%;margin:10px 20%></p>
                <ul>
                    <li>width、height<br>widthとheightは要素本体の横幅と縦幅です。text-alineや&lt;br>を使わない改行はこれをもとに行われます。
                    基本的には自動的に設定されますが指定する際にはこの二つがあまりにも小さすぎると要素の中身が要素からはみ出して表示されてしまうことに注意してください。width:～;、height: ～;で指定可能。</li>
                    <li>padding<br>paddingは要素本体の外側でborderの内側の余白を設定することが出来ます。基本的に枠線や下線の内側の余白を作るときに使います。padding: ～; で四方にpaddingを設定、 padding-top(left、right、bottom)で一方向のみに設定することが出来ます。</li>
                    <li>border<br>要素の内側と外側の境目です。枠線や下線を作るときに使います。border: 幅 種類 色;で指定できるので詳しい書き方は調べてみてください。</li>
                    <li>margin<br>要素の外側の余白です。他の要素との間に余白を作りたいときに使います。負の値を取ることが出来ますがレイアウトが崩れる原因にもなるので負の値は使わない方が良いです。</li>
                </ul>
                <p>そしてそれらの大きさの指定に使うのがpxなどの単位です。なんとなく使ってしまいがちですがそれぞれの単位の意味を考えて使いましょう。</p>
                <ul>
                    <li>px<br>pxは絶対的な単位なのでどのような媒体であっても大きさを変えたくないところに使うのがおすすめです。</li>
                    <li>vw、vh<br>vwとvhは相対的な値でそれぞれサイトが表示される画面の横幅と縦幅を参照します。スマホから見るかパソコンから見るかによって文字や写真の大きさをかえるレスポンシブデザインに便利です。</li>
                    <li>%<br>%は相対的な値でその要素本体の大きさを参照します。vwやvhを使うことで大体代用できます。</li>
                    <li>em、rem<br>emとremは相対的な値でそれぞれ親要素のフォントサイズ、サイト全体に適応されているフォントサイズを参照します。</li>
                </ul>
                <p>余白の調節に使うものと単位の紹介は以上です。これはあくまでも紹介なので気になることがあったら積極的に調べましょう。</p>
            </article>

            <article>
                <h2 id="6">displayの種類</h2>
                <hr size=10 color="black" class="hrLine">
                <p>要素の表示形式を設定するdisplayはpaddingやmarginと並んで重要なスタイルの一つです。基本的にdisplay:～;だけで指定できるのですが～にどれを選ぶかによって表示のされ方が全く異なるのでこの章では～の部分を紹介します。</p>
                <ul>
                    <li>display:block<br>この形式は最も基本的な形式で要素が縦に並んでいきます。要素と要素の間には必ず改行が入るのでこの形式のものを横ならべすることは基本的には出来ません。</li>
                    <li>display:inline<br>この形式では要素が横に並んでいきます。しかし幅や高さが指定できなかったりと様々な制約があるので特別な理由がない限り下のinline-blockを使うのが良いです。</li>
                    <li>display:inline-block<br>この形式では要素が横に並んでいき、幅や高さも指定できるので横並べをしたいときはこれを使いましょう。</li>
                    <li>display:none;<br>要素を表示されなくする形式です。あくまでも表示されないだけなので裏ではきちんと読み込まれています。</li>
                    <li>display:flex;<br>これも要素を横並びにする形式ですが様々な機能があり大量の要素を一律で横並べする時に便利です。少し書き方が特殊なので使うときはきちんと調べましょう。</li>
                </ul>
                <p>主に使うものはこの5つです。また、displayとは他にfloat:～;というのを使って要素を横ならべにすることが出来ます。</p>
            </article>

             <article>
                <h2 id ="7">演習問題(総復習)</h2>
                <hr size=10 color="black" class="hrLine">
                <p>以下のものを再現してみよう!(要素の中央そろえはmargin:0 auto;を書き、要素の横幅を指定すれば出来ます。</p>
                <div class="reset" style="border:1px solid black;margin:5px;width:100%;padding:5px">
                    <p style="display: inline-block; margin: 50px;">横並び1</p>
                    <p style="display: inline-block; margin: 50px;">横並び2</p>
                    <div style="padding: 20px; border: solid black 2px; margin: 0 auto; width: 50vw; text-align: center;">
                       <h1>この要素には枠線が付いています！</h1>
                    </div>
                </div>
                <p>解答は<nuxt-link to="#9">下の方</nuxt-link>にあります</p>
            </article>

            <article>
                <h2 id="8">おわりに</h2>
                <hr size=10 color="black" class="hrLine">
                <p>以上でHP講座第二回は終了です。htmlの書き方というよりcssの書き方中心になってしまい、内容的にも少し難しいのが多かったと思います。
                    講座内で何度も言っている通りこの講座内に書かれていることはあくまでも紹介であり「こんなことができるよ～」程度の道しるべにすぎません。
                    ぜひとも実際に自分で簡単なサイトを作ってみるなどして分からないところを自分で調べて行きながら経験を積んでいってください。
                </p>
            </article>

            <article>
                <h2 id="9">解答</h2>
                <hr size=10 color="black" class="hrLine">
                <p><nuxt-link to="#7">この問題</nuxt-link>の解答例です</p>
                <pre style="padding:2vw;background-color:#eeeeee">
                    &lt;!DOCTYPE html>
&lt;html lang="ja">
&lt;head>
  &lt;meta charset="UTF-8">
  &lt;style>
    p{
      display: inline-block;
      margin: 50px;
    }

    .waku{padding: 20px;
      border: solid black 2px;
      margin: 0 auto; 
      width: 50vw;
      text-align: center;
    }
  &lt;/style>
&lt;/head>
&lt;body>
  &lt;p>横並び1&lt;/p>
  &lt;p>横並び2&lt;/p>

  &lt;div class="waku">
    &lt;h1>この要素には枠線が付いています！&lt;/h1>
  &lt;/div>
&lt;/body>
&lt;/html>
                </pre>
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
              items:["はじめに","良く使うタグ(補足)","cssの外部化","cssとhtmlの対応","良く使うスタイル","padding,marginなどの関係性","displayの種類","演習問題(総復習)","おわりに","解答"]
            }
          },
        }
        </script>
