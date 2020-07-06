<template>
  <div id="app">
    <head>
    <!-- Fontawesome for icons CSS -->
    <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" />
    <link rel="icon" href="https://www.freepnglogos.com/uploads/twitter-logo-png/twitter-logo-vector-png-clipart-1.png">
    </head>


    <div class = "flexbox-container justify-content-center">
        <div class="flexbox-sidebar flex-column d-none d-lg-block d-md-block d-sm-block" id = "sidebar">
            <div class = "d-flex p-2">
                <a href="#" class = "logo"><span class = "fa fa-twitter"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-home" style = "color:#1DA1F2"></span><b style = "color:#1DA1F2">Home</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-hashtag"></span><b>Explore</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-bell-o"></span><b>Notifications</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-envelope-o"></span><b>Messages</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-bookmark-o"></span><b>Bookmarks</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-list-ul"></span><b>Lists</b></a>
            </div>

            <div class = "d-flex p-2">
                <a href="#"><span class="fa fa-user-o"></span><b>Profile</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-caret-down"></span><b>More</b></a>
            </div>

            <div class = "d-flex p-2 ">
                <button class="buttonSidebar"><b>Tweet</b></button>
            </div>

            <div class = "d-flex p-2 ">
                <button class="buttonSidebar" id = "sidepic">
                    <div class = "d-flex flex-row">
                        <div class = "d-flex p-1">
                        <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                        <div class = "d-flex p-1 flex-column align-items-start" style = "padding-top:20px;">
                            <div class = "d-flex" style = "max-height: 20px;">
                                <p class = "font-weight-bold  d-none d-md-block d-lg-block">
                                    Ronel
                                </p>
                            </div>

                            <div class = "d-flex">
                                <p class = "font-weight-bold text-secondary">
                                    @Ethan_Pag
                                </p>
                            </div>
                        </div>
                    </div>
                </button>
            </div>
        </div>



        <div class="flexbox-sidebar flex-column d-sm-none d-block" id = "sidebar">
            <div class = "d-flex p-2">
                <a href="#" class = "logo"><span class = "fa fa-twitter"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-home" style = "color:#1DA1F2"></span></a>
            </div>

            <div class = "d-flex p-2">
                <a href="#"><span class="fa fa-hashtag"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-bell-o"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-envelope-o"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-bookmark-o"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-list-ul"></span></a>
            </div>

            <div class = "d-flex p-2">
                <a href="#"><span class="fa fa-user-o"></span></a>
            </div>

            <div class = "d-flex p-2 ">
                <a href="#"><span class="fa fa-caret-down"></span></a>
            </div>

            <div class = "d-flex p-2 ">
            <button class="buttonSidebar"><i class="fa fa-pencil" aria-hidden="true"></i></button>
            </div>

            <div class = "d-flex p-2 ">
                <button class="buttonSidebar" id = "sidepic">
                    <div class = "d-flex flex-row">
                        <div class = "d-flex p-1">
                        <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                    </div>
                </button>
            </div>
        </div>



        <div class="flexbox-tweets d-flex flex-column">
            <div class = "d-flex wholetweet">
                <div class = "d-flex p-2"></div>
                <div class = "d-flex p-2">
                <div class = "d-flex p-2"><h3 class = "home">Home</h3></div>
            </div>
            </div>

            <div class = "d-flex flex-row wholetweet">
                <div class = "d-flex p-2">
                <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                <div class = "d-flex p-2 flex-column" style = "padding-top:20px;flex:1">
                    <div class = "d-flex" style = "width:100%;">
                        <textarea class="form-control" v-model= "NewTweet" rows="3" placeholder="What's happening?" style = "resize: none; width:100%; border:none"></textarea>
                    </div>

                    <div class = "d-flex flex-row">
                        <div class = "d-flex p-2">
                            <a href="#" class = "tweeticons"><i class="fa fa-picture-o" aria-hidden="true"></i></a>
                        </div>
                        <div class = "d-flex p-2">
                            <a href="#" class = "tweeticons"><i class="fa fa-file-video-o" aria-hidden="true"></i></a>
                        </div>
                        <div class = "d-flex p-2 d-none d-md-block">
                            <a href="#" class = "tweeticons"><i class="fa fa-bar-chart" aria-hidden="true"></i></a>
                        </div>
                        <div class = "d-flex p-2">
                            <a href="#" class = "tweeticons"><i class="fa fa-smile-o" aria-hidden="true"></i></a>
                        </div>
                        <div class = "d-flex p-2 d-none d-md-block">
                            <a href="#" class = "tweeticons"><i class="fa fa-calendar-o" aria-hidden="true"></i></a>
                        </div>
                        <div class = "d-flex p-2 ml-auto">
                            <button v-on:click="createTweet" class="buttonSidebar"><b>Tweet</b></button>
                        </div>
                    </div>
                </div>

            </div>

            <Tweet
            v-for="(tweet,index) in tweets"
            v-bind:key="tweet.id"
            v-bind:text="tweet.text"
            v-bind:thistweet="index"
            v-bind:edit="false"
            v-on:delete="deleteTweet"
            >
            </Tweet>


        </div>



        <div class="flexbox-rightsidebar flex-column d-none d-lg-block">
            <div class = "d-flex p-2">
                <textarea class="form-control" rows="1.5" placeholder="Search Twitter" style = "resize: none; width:100%; border:none; border-radius: 20px 20px 20px 20px;; background-color: #e6ecf0;"></textarea>
            </div>

            <div class = "d-flex p-2 flex-column" style = "background-color: #f5f8fa; border-radius:5%">
                <div class = "d-flex p-2"><h5 class = "home">Philippines trends</h5></div>



                <div class = "d-flex" style = "width:100%">
                    <div class = "d-flex flex-column" style = "width:100%">
                        <div class = "d-flex trending sidebardiv" style = "border-top:2px solid #e9eef2; width:100%;">
                            <p class = "sidebartext">1&nbsp;&#8231;&nbsp;Trending</p>
                        </div>
                        <div class = "d-flex trending sidebardiv" style = "border-bottom:2px solid #e9eef2; width:100%">
                            <p class = "sidebartext">ACSS&nbsp;Elections</p>
                        </div>
                    </div>
                </div>

                <div class = "d-flex" style = "width:100%">
                    <div class = "d-flex flex-column" style = "width:100%">
                        <div class = "d-flex trending sidebardiv" style = "width:100%;">
                            <p class = "sidebartext">2&nbsp;&#8231;&nbsp;Trending</p>
                        </div>
                        <div class = "d-flex trending sidebardiv" style = "border-bottom:2px solid #e9eef2; width:100%">
                            <p class = "sidebartext">Shopee&nbsp;Code&nbsp;League</p>
                        </div>
                    </div>
                </div>

                <div class = "d-flex" style = "width:100%">
                    <div class = "d-flex flex-column" style = "width:100%">
                        <div class = "d-flex trending sidebardiv" style = "width:100%;">
                            <p class = "sidebartext">3&nbsp;&#8231;&nbsp;Trending</p>
                        </div>
                        <div class = "d-flex trending sidebardiv" style = "border-bottom:2px solid #e9eef2; width:100%">
                            <p class = "sidebartext">Valorant&nbsp;Ranked</p>
                        </div>
                    </div>
                </div>

                <div class = "d-flex" style = "width:100%">
                    <div class = "d-flex flex-column" style = "width:100%">
                        <div class = "d-flex trending sidebardiv" style = "width:100%;">
                            <p class = "sidebartext">4&nbsp;&#8231;&nbsp;Trending</p>
                        </div>
                        <div class = "d-flex trending sidebardiv" style = "border-bottom:2px solid #e9eef2; width:100%">
                            <p class = "sidebartext">Project&nbsp;Revive</p>
                        </div>
                    </div>
                </div>


                <div class = "d-flex" style = "width:100%">
                    <div class = "d-flex flex-column" style = "width:100%">
                        <div class = "d-flex trending sidebardiv" style = "width:100%;">
                            <p class = "sidebartext">5&nbsp;&#8231;&nbsp;Trending</p>
                        </div>
                        <div class = "d-flex trending sidebardiv" style = "border-bottom:2px solid #e9eef2; width:100%">
                            <p class = "sidebartext">Twitch</p>
                        </div>
                    </div>
                </div>

                <div class = "d-flex p-2" style = "width:100%">
                    <a href="#" style = "color: #1DA1F2">Show More</a>
                </div>

            </div>






            <div class = "d-flex p-2"></div>

            <div class = "d-flex p-2 flex-column" style = "background-color: #f5f8fa; border-radius:5%">
                <div class = "d-flex p-2"><h5 class = "home">Who to follow</h5></div>

                <div class = "d-flex p-2" style = "border-top:2px solid #e9eef2; width:100%">
                        <div class = "d-flex flex-row">
                            <div class = "d-flex p-1">
                            <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                            <div class = "d-flex p-1 flex-column align-items-start" style = "padding-top:20px;">
                                <div class = "d-flex" style = "max-height: 20px;">
                                    <p class = "font-weight-bold  d-none d-md-block d-lg-block">
                                        Beard Boi
                                    </p>
                                </div>

                            <div class = "d-flex">
                                    <p class = "font-weight-bold text-secondary">
                                        @Man_Beard
                                    </p>
                                </div>
                            </div>


                            <div class = "d-flex flex-column align-self-center ">
                            <button class="followbutton ">
                                <a href="#" style = "color: #1DA1F2">Follow</a>
                            </button>
                        </div>

                        </div>
                </div>


                <div class = "d-flex p-2" style = "border-top:2px solid #e9eef2; width:100%">
                        <div class = "d-flex flex-row">
                            <div class = "d-flex p-1">
                            <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                            <div class = "d-flex p-1 flex-column align-items-start" style = "padding-top:20px;">
                                <div class = "d-flex" style = "max-height: 20px;">
                                    <p class = "font-weight-bold  d-none d-md-block d-lg-block">
                                        ??? Guy
                                    </p>
                                </div>

                            <div class = "d-flex">
                                    <p class = "font-weight-bold text-secondary">
                                        @Idk_man
                                    </p>
                                </div>
                            </div>


                            <div class = "d-flex flex-column align-self-center ">
                            <button class="followbutton ">
                                <a href="#" style = "color: #1DA1F2">Follow</a>
                            </button>
                        </div>

                        </div>
                </div>


                <div class = "d-flex p-2" style = "border-top:2px solid #e9eef2; border-bottom:2px solid #e9eef2;width:100%">
                        <div class = "d-flex flex-row">
                            <div class = "d-flex p-1">
                            <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                            <div class = "d-flex p-1 flex-column align-items-start" style = "padding-top:20px;">
                                <div class = "d-flex" style = "max-height: 20px;">
                                    <p class = "font-weight-bold  d-none d-md-block d-lg-block">
                                        Not Ethan
                                    </p>
                                </div>

                            <div class = "d-flex">
                                    <p class = "font-weight-bold text-secondary">
                                        @Not_Ethan
                                    </p>
                                </div>
                            </div>


                            <div class = "d-flex flex-column align-self-center ">
                            <button class="followbutton ">
                                <a href="#" style = "color: #1DA1F2">Follow</a>
                            </button>
                        </div>

                        </div>
                </div>

                <div class = "d-flex p-2" style = "width:100%">
                    <a href="#" style = "color: #1DA1F2">Show More</a>
                </div>

            </div>
        </div>

        
    </div> 
  </div>
</template>

<script>
import Tweet from "@/components/Tweet.vue"
import listweets from "@/assets/tweets.json"


export default {
  name: 'Twitter',
  components:{
      Tweet
  },
  data(){
        return{tweets:listweets.tweets,currentid:1050118621198921728}
  },methods:{
      deleteTweet(tweetIndex){
          this.tweets.splice(tweetIndex,1);
      },
      createTweet(){
          this.tweets.unshift({ id: (this.currentid+1), text: this.NewTweet })
          this.NewTweet = ""
          this.currentid = this.currentid+1
      },editTweet(wholeTweet){
        wholeTweet.edit = true
      }
  }
}
</script>

<style>

@import "https://fonts.googleapis.com/css?family=Helvetica%20Neue";
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap');

/*all text will have weight of 300*/
body {
    font-family: 'Helvetica Neue', sans-serif;
}

p {
    font-family: 'Helvetica Neue', sans-serif;
    font-weight: 300;
}

.flexbox-container{
	display:flex;
}

/*main container for left sidebar*/
.flexbox-sidebar{
	width: 200px;
	margin:10px;
	flex:.8;
}

/*main container for tweets middle flexbox*/
.flexbox-tweets{
	width: 200px;
	margin:10px;
	/*border:3px solid #333;*/
	min-width: 375px;
	min-height: 667px;
	flex:2.2;
}

/*main container for right sidebar*/
.flexbox-rightsidebar{
	width: 200px;
	margin:10px;
	flex:1.2;

}

/*all a elements in sidebar to be given this attribute*/
#sidebar div a{
	padding: 10px;
    font-size:1.3em;
    display: block;
}

/*hover color change effect*/
#sidebar div a:hover {
    color: #1DA1F2;
}

/*hover effect*/
a, a:hover, a:focus {
    color: inherit;
    text-decoration: none;
    transition: all 0.3s;
}

/*Formatting for icons*/
span {
 display: flex;
 width: 10px;
 padding-right: 40px;
}


/*special formatting for twitter logo*/
.logo{
    color: #1DA1F2;
    font-size:2em !important;
}

/*special formatting for icons in the twitter feed*/
.tweeticons{
    color: #1DA1F2;
    font-size:1.4em !important;

}

/*formatting for the tweet button on the sidebar*/
.buttonSidebar {
  background-color: #1DA1F2;
  color: white;
  text-align: center;
  cursor: pointer;
  border-radius: 20px 20px 20px 20px;
  width:100%;
  padding-top:10px;
  padding-bottom: 10px;
}

/*formatting for the "button" containing the profile picture+user+username in sidebar*/
.buttonSidebar {
  background-color: #1DA1F2;
  color: white;
  text-align: center;
  cursor: pointer;
  border-radius: 20px 20px 20px 20px;
  border-color:transparent !important;
  padding-top:8px;
  padding-bottom: 8px;
  padding-left: 20px;
  padding-right:20px;
}

/*change color upon hover in sidebar*/
.buttonSidebar:hover {
    background: #1992db;
}

/*special formatting for profile pictures*/
#profpic{
    border-radius:50%;
    width:60px;
    height:60px;
}

/*give tweet a very light-grey background*/
.wholetweet{
	border:1px solid #DCDCDC;
}

/*special formatting for left profile picture and on tweet above*/
#sidepic{
	padding-top:0px !important;
	padding-bottom: 0px !important;
	color:black;
	background-color: transparent !important;
	border-color:transparent !important;
}

.home{
  font-family: 'Roboto', sans-serif;
}

.sidebartext{
  color: #3b3f43;
}

.sidebardiv{
  max-height: 30px;
}

.followbutton{
  text-align: center;
  cursor: pointer;
  max-height: 30px;
  border-radius: 20px 20px 20px 20px;
  padding-left: 20px;
  padding-right:20px;
  border-color:#1DA1F2 !important;
}

</style>
