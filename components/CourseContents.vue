<template>
  <div class="containar" style="margin:0 5%;border:2px solid black;color:black">
    <div style="text-align:center;width:100%;"><p>▼目次▼</p></div>
    <nav class="row">  
      <nuxt-link v-for="(item,index) in items" v-bind:key="item.id" :to="'#'+index" class="col-md-6" style="color:black;text-indent:1em"><li>{{ item }}</li></nuxt-link> 
    </nav>
  </div>
</template>


<script>
export default {
  props: {
    items:{
      type:Array
    }
  },
}
</script>