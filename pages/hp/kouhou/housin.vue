<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole">
      <course-title title="広報HP講座の方針" subtitle="広報HP講座の順番と理由" date="2021/10/31" />
      <section>
        <h2 id="0">はじめに</h2>
        <hr size=10 color="black" class="hrLine">
        <p>これは広報係HP講座の方針についての説明です。広報HP講座一覧は<nuxt-link to="/#hp">こちら</nuxt-link>。</p>
      </section>
      <section>
        <h2 id="1">HP講座の最終目標</h2>
        <hr size=10 color="black" class="hrLine">
        <p>最終目標はnuxt.jsをGitHubで共同開発する事です。そしてその後としてDjangoを使ってもらおうと考えています。</p>
        <p></p>
      </section>
      <section>
        <h2 id="2">大切にしたいこと</h2>
        <hr size=10 color="black" class="hrLine">
        <p>読むと言うより実践することを中心としよう！というのが目標です。講座内の演習問題や<nuxt-link to="/hp/kouhou/boshu">講座・記事募集</nuxt-link>といったものを通じてこれを達成したいと考えています。</p>
      </section>
      <section>
        <h2 id="3">広報係HP講座の順番</h2>
        <hr size=10 color="black" class="hrLine">
        <div class="CourseOrder">
          <p style="background-color:orange">HTML</p>
          <p style="font-size:1em">↓</p>
          <p style="background-color:purple;color:white">GitHub</p>
          <p style="font-size:1em">↓</p>
          <p style="background-color:lightgreen">Nuxt.js</p>
          <p style="font-size:1em">↓</p>
          <p style="background-color:skyblue">（Django）</p>
        </div>
        <h3>それぞれの説明</h3>
        <ol class="ulstyle">
          <li>HTML<br>コードを書くやつです。HPの全ての始まり。<nuxt-link to="/hp/kouhou/course1">第一回HP講座</nuxt-link>。</li>
          <li>GitHub（<a href="https://github.com">https://github.com</a>）<br>共同開発するためのものです。バージョン管理が楽なのでGoogleドライブではなくこっちです。</li>
          <li>Nuxt.js（<a href="https://nuxtjs.org/">https://nuxtjs.org/</a>）<br>HTMLの派生です。導入が面倒ですがHPはこれで作った方がいいです。静的コンテンツです。</li>
          <li>Django（<a href="https://www.djangoproject.com/">https://www.djangoproject.com/</a>）<br>通信関係をPythonで動かします。動的コンテンツです。</li>
        </ol>
        <h3>意図</h3>
        <ol class="ulstyle">
          <li>なんでhtmlじゃなくてNuxt.jsを使うの？<br>ルート設定が簡単だからです。また、コンポーネントを利用することで見やすいコードができます。あとは…流行り？</li>
          <li>なぜ最初からNuxt.jsじゃないの？<br>Nuxt.jsはhtmlの派生です。Nuxt.jsはhtmlの一部を省略できるみたいな書き方なので、htmlが分からないと覚える事が多すぎてパンクします。まずは覚える事が少なく、汎用性が高いhtml講座を先にした方が良いと思いこのようにしました。</li>
          <li>途中でGitHubを挟むのはなぜ？<br>Nuxt.jsのプロジェクトを作成する時にGitHubアカウントを聞かれます。また、今後も使う可能性が高いものだからです。ただ、ここでつまずいてしまうくらいなら飛ばして貰って構わないと思っています。</li>
          <li>Djangoはhtml関係ないのになんで最後に持ってきたの？<br>一番大きな理由は僕ができないからです。また、Django単体では面白いことができないので最後にしました。</li>
        </ol>
      </section>
      <course-link-index type1="HP講座" type1link="/hp/" type2="by広報総務" type2link="/#hp" />
    </div>
  </div>
</template>

<style scoped>
.ulstyle li {
  margin-bottom: 10px;
}
article {
  margin-top: 40px;
}
h3 {
  margin-top: 20px;
}
.CourseOrder{
  text-align:center;
  background-color:#eeeeee;
  padding:20px;
}
.CourseOrder p{
  font-size: 2em;
}
</style>