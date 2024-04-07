<template>
    <navbar>
    </navbar>
    <router-view>
    </router-view>
  

</template>

<script>
  import Navbar from '../src/components/Navbar.vue'


  export default {
    components:{ 
      Navbar,
    },
    // created(){
    //   this.getPages();
      
      // this.$bus.$on('navbarLinkActivated',(index)=>{
      //   this.activePage = index;
      // })
    // },
    methods:{
      // async getPages(){
      //   let res = await fetch('pages.json')
      //   let data = await res.json();
      //   this.pages = data;
      // },
      pageCreated(pageObj){
        this.pages.push(pageObj);
      }
    }
  } 
</script>