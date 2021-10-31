<template>
  <div class="col-md-6 news">
    <a :href="link">
      <img :src="picture_name" :alt="picture_alt" style="width:100%">
      <p>{{ picture_alt }}</p>
    </a>
  </div>
</template>

<style scoped>
.news{
  padding:0px;
  margin:0px;
}
.news a{
  padding:0;
  margin:0;
  border:0;
}
.news img{
  padding:1vw;
}
.news p{
  color:black;
}
.news p:hover{
  color:#505050;
}
</style>

<script>
export default {
  props: [
    'link',
    'picture_name',
    'picture_alt',
  ],
}
</script>