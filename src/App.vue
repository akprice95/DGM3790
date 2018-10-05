<template>
 <div>
   <header>daHeader</header>
     <hr/>
 </div>

</template>
//adding comment to check gitKraken
<script>
import HelloWorld from './components/HelloWorld.vue'
import daHeader from './components/daHeader.vue'
import servers from'./components/servers.vue'
import serverDetails from './components/serverDetails.vue'
import daFooter from'./components/daFooter.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    daHeader,
    servers,
    serverDetails,
     daFooter
  
  },
  data () {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [{
        icon: 'bubble_chart',
        title: 'Inspire'
      }],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
