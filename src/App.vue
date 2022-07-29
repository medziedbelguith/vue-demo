<template>
<div>
<Header @changeTitle="changeText" :text="text"/>
</div>
</template>

<script>
import Header from "@/components/Header.vue"

export default {
  name: "App",
  components:{
    Header,
  },
  data(){
    return{
    text:"Ini adalah text dari app.vue"
    };
  },
  methods:{
    changeText(newText){
      this.text=newText;
    }
  }
};
</script>

<style>
</style>
