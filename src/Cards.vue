<template>
  <v-layout>
    <v-flex xs12 sm4 offset-sm3>

      <v-card>
        <v-card-media src="/public/vkhack.jpg" height="200px">
        </v-card-media>

        <div class="acounts">
          <div id="mount">
            <span class="friens"><b>{{ count }} друзей</b><br>идут</span><br>
          </div>
          <div class="avatars">
            <v-avatar>
              <img src="public/1.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/2.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/3.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/4.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/5.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/6.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/7.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/8.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/9.jpg" alt="John">
            </v-avatar>

            <v-avatar >
              <img src="public/10.jpg" alt="John">
            </v-avatar>
          </div>
        </div>
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">{{ nameCard }}</h3>
            <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
          </div>
        </v-card-title>
        <navbar></navbar>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Navbar from './Navbar.vue'
export default {

  data () {
    return {
      count: "15",
      nameCard: "Hello Vue",
      card_text: 'Lorem ipsum dolor sit amet, brute iriure accusata ne mea. Eos suavitate referrentur ad, te duo agam libris qualisque, utroque quaestio accommodare no qui. Et percipit laboramus usu, no invidunt verterem nominati mel. Dolorem ancillae an mei, ut putant invenire splendide mel, ea nec propriae adipisci. Ignota salutandi accusamus in sed, et per malis fuisset, qui id ludus appareat.'
    } 
  },
  components: {Navbar}
}
</script>

<style>
.card {
  background-color: white;
}
.acounts {
  position: relative;
  float: left;
  width: 100%;
  margin: 0;
  height: 78px;
  padding: 0;
  box-shadow: 0px 5px 7px -5px grey;
  padding: 5px;
}
.avatars {
  position: absolute;
  top: 0;
  bottom: 0;
  margin: auto 0;
  right: 0;

  float: left;
  padding: 0 10px;
  width: 84%;
  height: 48px;


  overflow-x: scroll;
  overflow-y: hidden;
  white-space: nowrap;

}
#mount { 
  display: table;
  float: left;
  width: 15%;
  height: 100%;
  padding: 0;
  text-align: center;
  border-right: 1px solid grey; 
  text-align: center;
}
.friens{
  display: table-cell;
  vertical-align: middle;
}
.avatar{
  margin: 0 5px;
}
::-webkit-scrollbar { 
  display: none; 
}

</style>