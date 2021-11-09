<template>
  <div class="containar" style="margin:0 5%;border:2px solid black;color:black">
    <div style="text-align:center;width:100%;"><p>▼目次▼</p></div>
    <ul class="row">  
      <nuxt-link v-for="(item,index) in items" v-bind:key="item.id" :to="'#'+index" class="col-md-6" style="color:black"><li>{{ item }}</li></nuxt-link> 
    </ul>
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