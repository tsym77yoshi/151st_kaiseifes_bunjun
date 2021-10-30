<template>
  <div class="col-md-6 news">
    <component
      :is="isInternalLink(link) ? 'nuxt-link' : 'a'"
      :to="isInternalLink(link) ? link : ''"
      :href="isInternalLink(link) ? '' : link"
    >
      <img :src="picture_name" :alt="picture_alt" style="width:100%">
    </component>
  </div>
</template>

<style>
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
</style>

<script>
export default {
  props: [
    'link',
    'picture_name',
    'picture_alt',
  ],
  methods: {
    isInternalLink (link) {
      return !/^https?:\/\//.test(link)
    }
  }
}
</script>