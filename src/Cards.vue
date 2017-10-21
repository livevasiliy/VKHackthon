<template>
  <v-layout>
    <v-flex xs4 v-for="i in 1" pl-3 pr-3 pt-3>
      <v-card>
      	<v-alert color="info" dismissible v-model="alert" transition="slide-y-transition">
			<div class="alertName">friend</div>
			<div class="alertFriendList">
				<div class="friend" v-for="i in 15">
					<div class="friend-img">
						<img src="" alt="">
					</div>
					<div class="friend-name">asdfsadf</div>
				</div>
			</div>
		</v-alert>
		<v-alert color="info" dismissible v-model="alert" transition="slide-y-transition">
			<!-- <div class="alertName">friend</div>
			<div class="alertFriendList">
				<div class="friend" v-for="i in 15">
					<div class="friend-img">
						<img src="" alt="">
					</div>
					<div class="friend-name">asdfsadf</div>
				</div>
			</div> -->
			<myFriend></myFriend>
		</v-alert>

        <v-card-media :src="logo" height="200px">
        </v-card-media>
        <div class="acounts">
          <div id="mount">            
            <v-btn block color="grey lighten-3" v-on:click="alert = true"><b>{{ count }} friends</b><br></v-btn>
          </div>
          <div class="avatars">
          <v-btn fab dark color="indigo" v-on:click="alert = true">
            <v-icon dark>add</v-icon>
          </v-btn>

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
          <div>{{ descrtp }} </div>
        </div>
      </v-card-title>
      <navbar></navbar>
    </v-card>
  </v-flex>
</v-layout>
</template>

<script>
import Navbar from './Navbar.vue';
import MyFriend from './MyFriend.vue';
export default {

  data () {
    return {
    	alert: false,
	    logo: "https://img05.rl0.ru/afisha/e560x-q80i/s4.afisha.ru/MediaStorage/e0/41/4bc4fddb54e74ce7a259080141e0.jpg",
	    nameCard: "Плакат эпохи революции", 
	    descrtp: "Плакат, пожалуй, шел рука об руку с революцией — после 1917 года именно он был рупором пропаганды и с успехом прививал малограмотному населению новые большевистские установки.",
	    count: "15",
	      
	    card_text: 'Lorem ipsum dolor sit amet, brute iriure accusata ne mea. Eos suavitate referrentur ad, te duo agam libris qualisque, utroque quaestio accommodare no qui. Et percipit laboramus usu, no invidunt verterem nominati mel. Dolorem ancillae an mei, ut putant invenire splendide mel, ea nec propriae adipisci. Ignota salutandi accusamus in sed, et per malis fuisset, qui id ludus appareat.'
    }
  },
  components: {Navbar, MyFriend}
}
</script>

<style>
	.card {
	  background-color: white;
	}
	.acounts {
	  background: #f5f5f5;
	  position: relative;
	  float: left;
	  width: 100%;
	  margin: 0;
	  height: 78px;
	  padding: 0;
	  box-shadow: 0px 5px 7px -5px grey;
	}
	.avatars {
	  position: absolute;
	  top: 0;
	  bottom: 0;
	  margin: auto 0;
	  right: 0;

	  float: left;
	  padding: 0 10px;
	  width: 73%;
	  height: 48px;



	  overflow-x: scroll;
	  overflow-y: hidden;
	  white-space: nowrap;
	}
	.avatars>.btn{
	  margin: 0 5px;
	  width: 48px;
	  height: 48px;
	  box-shadow: none;
	  }
	#mount { 
	  display: table;
	  float: left;
	  width: 15%;
	  height: 100%;
	  padding: 0;
	  text-align: center;
	  position: relative;
	    z-index: 10;
	}
	#mount>.btn{
	  box-shadow: none;
	  height: 100%;
	  margin: 0;
	  text-transform: lowercase;
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
	.alert{
		position: absolute;
	    z-index: 11;
	    top: -4px;
	    height: 100%;
	    width: 100%;
	}
	.alert>div{
		width: 100%;
		overflow: scroll;
	}
	.alertName{
		margin-bottom: 10px;
	}
	.friend{
		width: 100%;
		height: 90px;
		padding: 10px 0;
		box-shadow: 0px 1px 0px 0px darkslategrey;
	}
	.friend-img{
		float: left;
		width: 70px;
		height: 100%;
		border-radius: 50%;
    	background-color: yellow;
	}
	.friend-name{
		height: 100%;
		float: left;
		line-height: 70px;
		margin-left: 20px;
	}

</style>