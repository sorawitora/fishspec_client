<!----------Make By YourName---------------->
 <template>
  <div id="app">
       <Navbar/>
    <router-view/>
  </div>
</template>

  <script>
    import { get,sync,call } from "vuex-pathify"; 
    import Navbar from '@/components/Shere/Navbar.vue'
export default {
  name: 'Root',
  /*-------------------------Load Component---------------------------------------*/
  components: {
Navbar
  },
  /*-------------------------Set Component---------------------------------------*/
props:{

},
  /*-------------------------DataVarible---------------------------------------*/
  data() {
  return {

    };
  }, 
  /*-------------------------Run Methods when Start this Page------------------------------------------*/
   async mounted() {
  /**** Call loading methods*/
      this.load(); 
  },
  /*-------------------------Run Methods when Start Routed------------------------------------------*/
   async beforeRouteEnter(to, from, next) { 
    next()
  },
  /*-------------------------Vuex Methods and Couputed Methods------------------------------------------*/
  computed:{

},
  /*-------------------------Methods------------------------------------------*/
methods:{
  /******* Methods default run ******/
  load:async function(){
}
},
  }
</script>