<template>
  <div style="background-color:rgb(220,220,220);">
    <div class="whole">
      <course-title title="タイトル" subtitle="サブタイトル" date="2021/11/12"/><!--タイトル等-->
      <course-contents :items="items" /><!--目次・無くてもよい分量なら不要-->
      <section>
        <!--idは目次で利用しています-->
        <h2 id="0">はじめに</h2>
        <hr size=10 color="black" class="hrLine">
        <!--h2とhrの下線で作っています-->

        <p>この章で語ります・連絡先として四桁くらいはどこかで書くといいかも</p>
      </section>
      <section>
        <h2 id="1">第二章</h2>
        <hr size=10 color="black" class="hrLine">
        <pre style="padding:2vw;background-color:#eeeeee;">
&lt;!DOCTYPE html>
&lt;html>
  &lt;head>
    &lt;meta charset="utf-8">
  &lt;/head>
  &lt;body>
    &lt;!-- この下から書き始める -->

  &lt;/body>
&lt;/html></pre>
        <p>テキストテキスト</p>
      </section>
      <!-- シリーズものにするなら使ってください・初回の時はbeflink=""とbeftitle自体をなくしてください（aftlinkも同じ感じで） -->
      <CourseLink beflink="/course1" beftitle="第一回○○" aftlink="/hp/coursescourse3" afttitle="第三回○○" index="HP講座一覧" indexlink="/hp/courses/other" />
      <!-- 分類・必須 -->
      <course-link-index type1="HP講座" type1link="/hp/index" type2="その他" type2link="/hp/index#other" />
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
      items:["はじめに","第二章"]
    }
  },
}
</script>