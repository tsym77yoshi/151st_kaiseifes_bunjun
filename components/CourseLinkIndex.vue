<template>
  <nav style="margin-top:40px">
    <p style="font-size:1.3em">分類：<nuxt-link :to="type1link">#{{ type1 }}</nuxt-link> <nuxt-link :to="type2link">#{{ type2 }}</nuxt-link></p>
  </nav>
</template>


<script>
export default {
  props: [
    'type1',
    'type1link',
    'type2',
    'type2link',
  ],
}
</script>