<template>
 <div>
   <header>header</header>
     <hr/>
 </div>

</template>
//adding comment to check gitKraken
<script>
import HelloWorld from './components/HelloWorld'
import daHeader from './components/daHeader'
import servers from'./components/servers'
import serverDetails from './components/serverDetails'
import daFooter from'./components/daFooter'

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
