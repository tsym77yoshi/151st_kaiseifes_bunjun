<template>
  <div class="nav_back">
    <img src="~assets/icon.png" alt="文準アイコン" style="height:30px;margin:0px">
    <p class="nav_title"><u>151st文化祭準備委員会</u></p>
    <span class="nav_links" style="float:right;">
      <nuxt-link to="/"><p>ホーム</p></nuxt-link>
      <nuxt-link to="/report/"><p>文準通信</p></nuxt-link>
      <nuxt-link to="/hp/kouhou/course1/"><p>HP講座</p></nuxt-link>
      <nuxt-link to="/movie/course1/"><p>動画講座</p></nuxt-link>
    </span>
  </div>
</template>

<style>
.nav_back{
  position:relative;
  padding:0 5px 0;
  width:100%;
  background-color:#F48441;
  z-index:10;
}
.nav_back p{
  font-size:20px;
  padding:5px 5px 0px;
}
.nav_title{
  display: inline-block;
  padding:5px;
  max-width:600px;
}
.nav_links p{
  display: inline-block;
}
.nav_links a{
  color:black;
  padding:0 0.5vw;
}
.nav_links a:hover{
  color: #505050;
}
@media screen and (max-width: 639px) {
  .nav_title {
    display:none;
  }
  .nav_links{
    margin-left: auto;
  }
  .nav_links p{
    padding-top:0px;
  }
}
</style>