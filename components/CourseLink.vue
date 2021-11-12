<template>
  <div class="containar">
    <h2>講座リンク</h2>
    <hr size=10 color="black" class="hrLine">
    <div class="row" style="text-align:center;vertical-align: middle;">
      <nuxt-link v-if="beflink" :to="beflink" class="col-4"><div class="flame"><p>[前回]<br>{{ beftitle }}</p></div></nuxt-link>
      <div v-else class="col-4"><div class="flamed"><p>[前回]<br>この記事が最初です</p></div></div>
      <nuxt-link :to="indexlink" class="col-4"><div class="flame"><p>[一覧]<br>{{ index }}</p></div></nuxt-link>
      <nuxt-link v-if="aftlink" :to="aftlink" class="col-4"><div  class="flame"><p>[次回]<br>{{ afttitle }}</p></div></nuxt-link>
      <div v-else class="col-4"><div class="flamed"><p>[次回]<br>この記事が最新です</p></div></div>
    </div>
  </div>
</template>

<style scoped>
.flame{
  margin:2px;
  border:1px solid black;
  background-color: #f9f9f9;
  height:70px;
  color:black;
}
.flamed{
  margin:2px;
  border:1px solid grey;
  background-color: #f9f9f9;
  color:grey;
  height:70px;
}
</style>

<script>
export default {
  props: [
    'beflink',
    'beftitle',
    'aftlink',
    'afttitle',
    'index',
    'indexlink',
  ],
}
</script>