<template>
  <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-card-media src="/public/vkhack.jpg" height="200px">
        </v-card-media>
        <div class="acounts">
      <div id="mount">
        <span class="friens"><b>{{ count }} друзей</b><br>идут</span><br>
      </div>
      <div class="avatars">
        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>

        <v-avatar class="indigo">
          <v-icon dark>account_circle</v-icon>
        </v-avatar>
      </div>
    </div>
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">{{ nameCard }}</h3>
              <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
            </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
  export default {

    data () {
      return {
        count: "15",
        nameCard: "Hello Vue",
        card_text: 'Lorem ipsum dolor sit amet, brute iriure accusata ne mea. Eos suavitate referrentur ad, te duo agam libris qualisque, utroque quaestio accommodare no qui. Et percipit laboramus usu, no invidunt verterem nominati mel. Dolorem ancillae an mei, ut putant invenire splendide mel, ea nec propriae adipisci. Ignota salutandi accusamus in sed, et per malis fuisset, qui id ludus appareat.'
      } 
    }
  }
</script>

<style>
  .card {
    background-color: white;
  }
  .acounts {

    float: left;
    width: 100%;
    margin: 0;
    padding: 0;
    box-shadow: 0px 5px 7px -5px grey;
    padding: 5px;
  }
  .avatars {
    float: left;
    padding: 0 10px;
    margin: 0;
    width: 85%;
    height: 48px;
    

    overflow-x: scroll;
    overflow-y: hidden;
    white-space: nowrap;

  }
  #mount { 
      float: left;
      width: 15%;
      height: 100%;
      margin: 0;
      padding: 0;
      text-align: center;
      border-right: 1px solid grey; 
      text-align: center;
   }
   
   .avatar{
        margin: 0 5px;
   }
::-webkit-scrollbar { 
    display: none; 
}

</style>