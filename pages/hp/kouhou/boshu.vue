<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole indent">
      <course-title title="HP講座募集" subtitle="HP講座募集について" date="2021/11/09"/>
      <course-contents :items="items" />
      <article>
        <h2 id="0">はじめに</h2>
        <hr size=10 color="black" class="hrLine">
        <p></p>
      </article>
      <article>
        <h2 id="1">形式</h2>
        <hr size=10 color="black" class="hrLine">
        <h3>html</h3>
        <p>Googleドライブやメールで送ってください。Nuxt.js化して上げます。写真とかも忘れずにつけてください（動画の場合はYouTube埋込みを使います。動画と埋込みコードリンク抜きをコード内に入れてください）</p>
        <h3>Nuxt.js</h3>
        <p>GoogleドライブでもGitHubでもOKです。写真等は上と同じです。</p>
        <h3>PDFなどその他形式</h3>
        <p>HPの講座作成はHPを書く経験も兼ねているのでこの形式ではなく上の2つのどちらかでお願いします。</p>
      </article>
      <article>
        <h2 id="2">内容</h2>
        <hr size=10 color="black" class="hrLine">
        <p>〇〇苦労したとか〇〇かっこよくない？とかそんな感じで大丈夫です。（例：リンク）もちろん完全版でもありがたいです。</p>
        <h3>分類（※10月31日現在）</h3>
        <p>HTML/GitHub/Nuxt.js(＆boostrap)/Django/デザイン/Figma/SEO/その他</p>
        <h3>特に募集中の記事</h3>
        <p>書くことが思いつかないという人は是非この下の話題を選んでみてください</p>
        <ol>
          <li>HTMLのheadの中に書くもの</li>
          <li>GitHubの理論（とか色々！）</li>
          <li>Django（第6回書きたい人は連絡お願いします）</li>
          <li>Figma</li>
          <li>SEO対策</li>
          <li>おすすめのデザイン（classも入れて）</li>
        </ol>
        <p>その他、思いついたことがあったら連絡お願いします。</p>
      </article>
      <article>
        <h2 id="3">注意事項</h2>
        <hr size=10 color="black" class="hrLine">
        <p>基本、このホームページに掲載します。しかし、文化祭全体のHPにも載せる可能性があります。また、来年以降も使う可能性があります。また、<u>ネット上に公開している</u>ので名前や写真を掲載する場合は<u>保護者の許可を取るよう</u>にお願いします。そして不適切な内容を入れるのはやめてください。僕が確認した上で、顧問の先生にも確認していただくことになるので注意してください。</p>
      </article>
      <article>
        <h2 id="4">送り先</h2>
        <hr size=10 color="black" class="hrLine">
        <p style="text-indent:0;">メールかDiscordにあげるということ・そして場合によっては本体を添付してください。GitHubのみにするのはやめてください。注意事項を確認するためです。</p>
        <ol class="clearnum" style="overflow:hidden">
          <li>メールアドレス：</li>
          <li>Discord：tsym_4745#1731（広報SC山下のアカウント）</li>
          <li>GitHub：<a href="https://github.com/tsym77yoshi/151st_kaiseifes_bunjun">https://github.com/tsym77yoshi/151st_kaiseifes_bunjun</a>（追加先はhpの各分類の下、kouhou外）</li>
        </ol>
        <p style="text-indent:0;">※返信遅くなったらすみません</p>
      </article>
      <article>
        <h2 id="5">その他</h2>
        <hr size=10 color="black" class="hrLine">
        <p>何か質問とか修正とかがあればdiscordかメールにお願いします。GitHubでの連絡方法は分かりません⊂( *･ω･ )⊃。HP担当の4桁番号：4745　4846</p>
      </article>
      
    </div>
  </div>
</template>

<style scoped>
.ulstyle li {
  margin-bottom: 10px;
}
</style>

<script>
import { defineComponent } from '@vue/composition-api'
import CourseContents from '../../../components/CourseContents.vue'

export default {
  components: { CourseContents },
  data (){
    return{
      items:["はじめに","形式","内容","注意事項","送り先","その他"]
    }
  },
}
</script>