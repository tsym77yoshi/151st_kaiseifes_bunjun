<template>
  <div>
    <hr width=100% size=10>
    <img src="~assets/table.svg" alt="・" style="height:40px;padding:0">
    <h1 style="display: inline-block;margin-bottom:20px">{{ title }}</h1>
    <p style="float:right;"><img src="~assets/access_time.svg" alt="T" style="height:1em;padding:0">{{ date }}</p>
    <p>{{ subtitle }}</p>
    <hr width="100%" size=10>
  </div>
</template>


<script>
export default {
  props: [
    'title',
    'date',
    'subtitle',
  ],
}
</script>