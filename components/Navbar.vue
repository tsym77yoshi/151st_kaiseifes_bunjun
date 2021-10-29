<template>
  <div class="nav_back">
    <div style="text-align:center">
      <img src="~assets/icon.png" alt="文準アイコン" style="height:35px;margin:0px">
      <p class="nav_title"><u>151s文化祭準備委員会</u></p>
      <div class="nav_links">
        <a href="https://151st-kaiseifes-bunjun.vercel.app/"><p>ホーム</p></a>
        <a href="https://151st-kaiseifes-bunjun.vercel.app/"><p>HP講座</p></a>
        <a href="https://151st-kaiseifes-bunjun.vercel.app/"><p>動画講座</p></a>
      </div>
    </div>
  </div>
</template>

<style>
.nav_back{
  position:relative;
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
.nav_links{
  display: inline-block;
}
.nav_links p{
  display:inline-block;
}
.nav_links a{
  color:black;
}
.nav_links a:hover{
  color: #505050;;
}
</style>