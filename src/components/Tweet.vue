<template>
    <div class = "Tweet">
            <div class = "d-flex flex-row wholetweet">
                <div class = "d-flex p-2">
                <img src="https://www.calwestern.com/wp-content/uploads/2017/12/person-3.png" alt="user" id = "profpic" style = "height:55px;width:55px"></div>
                <div class = "d-flex p-1 flex-column align-items-start" style = "padding-top:20px;">
                    <div class = "d-flex flex-column"> 
                        <div class = "d-flex" style = "max-height: 20px;">
                            <p class = "font-weight-bold  d-none d-md-block d-lg-block">Ronel   &nbsp;</p>
                            <p class = "font-weight-bold text-secondary">@Ethan_Pag &nbsp;</p>
                            <p class = "font-weight-bold text-secondary">&#8231;&nbsp;2m </p>
                        </div>
                        <div class = "d-flex p-1" v-if="edit==false">
                            <p>
                                {{ text }}
                            </p>
                        </div>

                        <div class = "d-flex p-1" v-else>
                            <textarea class="form-control" rows="3" placeholder="What's happening?" style = "resize: none; width:100%; border:none"></textarea>
                        </div>

                        <div class = "d-flex flex-row justify-content-around">
                            <div class = "d-flex p-2">
                                <i class="fa fa-comment-o" aria-hidden="true"></i>
                            </div>
                            <div class = "d-flex p-2">
                                <i class="fa fa-retweet" aria-hidden="true"></i>
                            </div>
                            <div class = "d-flex p-2">
                                <i class="fa fa-heart-o" aria-hidden="true"></i>
                            </div>
                            <div class = "d-flex p-2">
                                <button v-on:click="$emit('delete', thistweet)" style = "background-color:transparent; border-color:transparent;"><i class="fa fa-trash" aria-hidden="true"></i></button>
                            </div>
                            <div class = "d-flex p-2">
                                <button v-on:click="showEdit" style = "background-color:transparent; border-color:transparent;"><i class="fa fa-pencil-square-o" aria-hidden="true"></i></button>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
    </div>
</template>


<script>

export default {
    name: "Tweet",
    props:{
        text: String,
        thistweet:Number,
        // editText:String
        // edit:Boolean,
    },data(){
        return{
                edit:false,
                editText:""
        }
  },
  methods:{
    //   showEdit(){
    //       edit = true
    //   }
  }
}
</script>
