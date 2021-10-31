<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole indent">
      <img src="~assets/table.svg" alt="・" style="height:40px">
      <h1 style="display: inline-block;margin-bottom:20px">動画講座第一回</h1>
      <p style="text-indent:0">動画編集のススメ</p>
      <article>
        <h2>〇はじめに</h2>
        <p>これは来年の文化祭で参団に積極的に関わりたいと思っている方に向けた動画講座です。参団と動画は全く関係がないように思うかもしれませんが、150thではいくつかの参団が紹介動画を作っています。例えば、今年大好評だった参団「バランスアクションVR」は以下の動画を作成していました。</p>
        <blockquote class="twitter-tweet" data-lang="ja" data-dnt="true"><p lang="ja" dir="ltr">企画紹介<br><br>バランスアクション!VR <a href="https://twitter.com/VrRunning?ref_src=twsrc%5Etfw">@vrrunning</a><br>文化祭で、話題のVRアトラクションが遂に出た！近未来の世界でビルとビルとを横断して、飛行して…もっとリアルに、より直にVRを体感しよう！ <a href="https://t.co/Gbwnu1CNBX">pic.twitter.com/Gbwnu1CNBX</a></p>&mdash; 150th開成祭 (@kaisei_festival) <a href="https://twitter.com/kaisei_festival/status/1439215012803801094?ref_src=twsrc%5Etfw">2021年9月18日</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
        <p>皆さんもこんなかっこいい紹介動画を作ってみたいと思いませんか？そこで、この講座では動画編集をやったことがない方のために、0から編集技術を教えていきます。（筆者もまだまだ初心者なので、温かい目で見ていただけると幸いです。）</p>
      </article>
      <article>
        <h2>〇動画の作り方</h2>
        <p style="text-indent: 0;">動画の作り方は大きく次の２つに分けられます。</p>
        <ol class="clearnum">
          <li>① 素材（写真や映像など）を主軸にして作る方法</li>
          <li>② 動画編集ソフトで作ったパーツ（図形や文字など）を主軸にして作る方法</li>
        </ol>
        <p>比較的簡単に動画が作れるのは①の方法なので、動画編集が初めてだという方には①をお勧めします。しかし、この方法には動画の質が素材の質に左右されるという短所もあり、良い動画を作るためには編集技術だけでなく、カメラの技術やあるいは絵を描く技術といった他の技術が求められます。一方、②の方法では編集技術さえあれば他は何もいりません。そのため、この際動画編集を極めたいという方は②をお勧めします。ちなみに、先ほどの「バランスアクションVR」の紹介動画は（最後のシーンを除いて）②の方法で作られています</p>
      </article>
      <article>
        <h2>〇動画編集ソフトについて</h2>
        <p>この講座で扱う動画編集（加工）ソフトはAviUtl, Adobe Premire Pro, Adobe Affter Effects, DaVinci Resolveの4つです。(筆者が主に使っているのはAviUtlです)</p>
        <p>このうち、Adobe Premire Pro, Adobe Affter Effects はAdobeに加入していないと使えませんが、全てのOSに対応しています。一方、AviUtlはWindowsにしか対応していませんが、無料で使用することができます。また、Davinci Resolveは無料で、かつWindows、Mac、Linuxのすべてに対応しています。（ただし、PCに高いスペックが求められます。）</p>
        <p style="text-indent: 0;">まとめると、</p>
        <ul>
          <li>Adobeに加入している→Adobe Premire Pro, Adobe Affter Effects がおすすめ</li>
          <li>Adobeに加入していない、かつWindows→AviUtl がおすすめ</li>
          <li>Adobeに加入していない、かつMac、Linux→DaVinci Resolveがおすすめ</li>
        </ul>
        <p style="text-indent: 0;">となります。</p>
        <p style="text-indent: 0;">ということで、次の章では各編集ソフトのインストール方法について解説します。</p>
      </article>
      <article>
        <h2>〇編集ソフトのダウンロード・インストール方法</h2>
        <article>
          <h3>1. AviUtl（参考：<a href="https://aviutl.info/intro/">https://aviutl.info/intro/</a>）</h3>
          <ol class="clearnum">
            <li>① 次のリンクにアクセスします：<a href="http://spring-fragrance.mints.ne.jp/aviutl/">http://spring-fragrance.mints.ne.jp/aviutl/</a></li>
            <li>② 本体と拡張編集プラグインの最新版をダウンロードします</li>
            <li>③ ダウンロードした本体（aviutl110.zip）とプラグイン（exedit93rc1.zip）のファイルを展開し、プラグインのフォルダ（exedit93rc1）内にある全ファイルを本体フォルダ（aviutl110）の中に移動します</li>
          </ol>
          <p>これでインストールは完了です。AviUtlフォルダの中にある「aviutl.exe」をダブルクリックすることでソフトを起動できます。</p>
          <p style="text-indent: 0">（重要な補足）</p>
          <ul>
            <li>様々な形式の動画を読み込むためには「L-SMASH Works」という入力プラグインを入れましょう。またその際「ファイル」→「環境設定」→「入力プラグインの優先度の設定」から「L-SMASH Works」を一番下に移動させましょう。（詳しくは<a href="https://aviutl.info/l-smash-works/">https://aviutl.info/l-smash-works/</a>を参照してください）</li>
            <br>
            <li>MP4形式（Youtubeなどの標準規格）での出力を可能にするプラグイン「x264guiEx」をダウンロードしましょう。（詳しくは<a href="https://aviutl.info/x264guiex-tokutyou/">https://aviutl.info/x264guiex-tokutyou/</a>を参照してください）</li>
          </ul>
        </article>
        <article>
          <h3>2.Adobe Premire Pro, Adobe Affter Effects</h3>
          <p style="text-indent: 0">どちらか片方でもいいですが、できれば両方インストールしましょう。</p>
          <ol class="clearnum">
            <li>① Adobe Creative Cloudを開きます</li>
            <li>② Adobe Premire Pro, Adobe Affter Effectsそれぞれのインストールボタンを押します</li>
          </ol>
          <p style="text-indent: 0">以上でインストールは完了です。</p>
        </article>
        <article style="overflow:hidden;">
          <h3>3.DaVinci Resolve（参考：<a href="https://udemy.benesse.co.jp/design/movie/how-to-davinci-resolve.html">https://udemy.benesse.co.jp/ design/movie/how-to-davinci-resolve.html</a>）</h3>
          <ol class="clearnum">
            <li>① 次のリンクにアクセスします：<a href="https://www.blackmagicdesign.com/jp/products/davinciresolve/">https://www.blackmagicdesign.com/jp/products/davinciresolve/</a></li>
            <li>② 「今すぐダウンロード」ボタンを押し、左上の「DaVinch Resolve 17」の中の自分のOSと同じものを選択します。</li>
            <li>③ 個人情報を登録し、ダウンロードします。</li>
            <li>④ ダウンロードしたZIPファイルを展開し、インストーラーを立ち上げます。</li>
            <li>⑤ インストールボタンを押し、後は流れに沿って進んでください。</li>
          </ol>
          <p style="text-indent: 0">以上でインストールは完了です。</p>
          <p style="text-indent: 0">（補足）<br>デフォルトの言語設定は英語となっていますが、日本語に直すこともできます。（詳しくは<a href="https://udemy.benesse.co.jp/design/movie/how-to-davinci-resolve.html">https://udemy.benesse.co.jp/design/movie/how-to-davinci-resolve.html</a>を参照してください。）</p>
        </article>
      </article>
      <article>
        <h2>〇各ソフトの操作方法について</h2>
        <p>詳しくは次回解説しますが、ダウンロードして何もできないというのは悲しいと思うので、いくつか有用なサイトを載せておきます。（有用すぎて次回からの講座いらないかも…）</p>
        <ul class="ulstyle" style="overflow:hidden;">
          <li>「AviUtlの易しい使い方」（<a href="https://aviutl.info/kyoukasyo/">https://aviutl.info/kyoukasyo/</a>）…AviUtlの教科書的存在</li>
          <li>「Premire Proチュートリアル」（<a href="https://helpx.adobe.com/jp/premiere-pro/tutorials.html">https://helpx.adobe.com/jp/premiere-pro/tutorials.html</a>）…Adobe公式さんのチュートリアル</li>
          <li>「After Effectsチュートリアル」（<a href="https://helpx.adobe.com/jp/after-effects/tutorials.html">https://helpx.adobe.com/jp/after-effects/tutorials.html</a>）…Adobe公式さんのチュートリアル</li>
          <li>「DaVinci Resolveの使い方」（<a href="https://udemy.benesse.co.jp/design/movie/how-to-davinci-resolve.html">https://udemy.benesse.co.jp/design/movie/how-to-davinci-resolve.html</a>）</li>
          <li>「DaVinch-Resolve-17-Beginners-Guide」（<a href="https://documents.blackmagicdesign.com/UserManuals/DaVinci-Resolve-17-Beginners-Guide.pdf?_v=1623283767000">https://documents.blackmagicdesign.com/UserManuals/DaVinci-Resolve-17-Beginners-Guide.pdf?_v=1623283767000</a>）…公式さんが出しているDaVinci Resolveの教科書的なもの（但し、英語版なので日本人のYoutubeチャンネル（<a href="https://www.youtube.com/channel/UCY3J0X26AAeqIijVE1kANIw/featured">https://www.youtube.com/channel/UCY3J0X26AAeqIijVE1kANIw/featured</a>）の解説と合わせて見るのがおすすめ）</li>
        </ul>
      </article>
      <article>
        <h2>〇おわりに</h2>
        <p>いかがでしたか。今回の内容じゃ物足りないという方はぜひ上に挙げたサイトで操作方法を覚えて、Youtubeなどにアップロードされているチュートリアルをガンガンこなしていってください。こなした数だけきっと力になります。</p>
      </article>
    </div>
  </div>
</template>

<style scoped>
.ulstyle li {
  margin-bottom: 10px;
}
h3 {
  margin-top: 20px;
}
</style>