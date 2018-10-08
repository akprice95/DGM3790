<template>


  <v-layout row>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-toolbar color="black" dark>
          <v-icon>build</v-icon>
          

          <da-header>Inbox</da-header>

          <v-spacer></v-spacer>
        </v-toolbar>

        <v-list two-line>
          <template v-for="(item, index) in items">
            <v-subheader
              v-if="item.header"
              :key="item.header"
            >
              {{ item.header }}
            </v-subheader>

            <v-divider
              v-else-if="item.divider"
              :inset="item.inset"
              :key="index"
            ></v-divider>

            <v-list-tile
              v-else
              :key="item.title"
              avatar
            >
              <v-list-tile-avatar>
                <img :src="item.avatar">
              </v-list-tile-avatar>

              <v-list-tile-content>
                <v-list-tile-title v-html="item.title"></v-list-tile-title>
                <v-list-tile-sub-title v-html="item.subtitle"></v-list-tile-sub-title>
              </v-list-tile-content>
            </v-list-tile>
             <template>

               
</template>


          </template>

          
        </v-list>
      </v-card>
      <template>
  <daFooter class="pa-3">
    <v-spacer></v-spacer>
    <div>&copy; {{ new Date().getFullYear() }}</div>
  </daFooter>
</template>
    </v-flex>

    
  </v-layout>


  
</template>
//adding comment to check gitKraken
<script>
import HelloWorld from './components/HelloWorld.vue'
import daHeader from './components/daHeader.vue'
import servers from'./components/servers.vue'
import serverDetails from './components/serverDetails.vue'
import daFooter from'./components/daFooter.vue'
import daFooterVue from './components/daFooter.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    daHeader: daHeader,
    servers,
    serverDetails,
     daFooter
  
  },
    data () {
      return {
        items: [
          {
            avatar: 'https://openclipart.org/download/89245/kuba-icon-ok.svg',
            title: 'Server #1',
            subtitle: "This server is up and running"
          },
          { divider: true, inset: true },
          {
            avatar: 'https://openclipart.org/download/89245/kuba-icon-ok.svg',
            title: 'Server #2',
            subtitle: "This server is up and running"
          },
          { divider: true, inset: true },
          {
            avatar: 'https://openclipart.org/download/89245/kuba-icon-ok.svg',
            title: 'Server #3',
            subtitle: "This server is up and running"
          },
          { divider: true, inset: true },
          {
            avatar: 'https://openclipart.org/download/307313/1538154540.svg',
            title: 'Server #4',
            subtitle: "This server needs some attention!!!"
          },
           { divider: true, inset: true },
          {
            avatar: 'https://openclipart.org/download/89245/kuba-icon-ok.svg',
            title: 'Server #5',
            subtitle: "This server is up and running"
          },
          
        ]
      }
    }
  }
  
</script>






