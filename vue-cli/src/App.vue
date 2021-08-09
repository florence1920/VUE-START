<template>
    <div>
        <app-header 
          v-bind:send="str" v-bind:send2="str2"
          v-on:renew="renewStr2"
        ></app-header>
    </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
export default {
  components: { 
    'app-header' : AppHeader
  },
  data: function(){
    return {
      str: 'Header',
      str2: 'Header2'
    }
  },
  methods:{
    renewStr2 : function(){
      this.str2 = 'hello'
    }
  }
  
}
</script>

<style>

</style>