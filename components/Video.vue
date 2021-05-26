<template>
    <div>
         <b-card :img-src="video.img" class="mb-2">
          <img class="user" src="../assets/img/user.png" alt="" />
          <p class="time">{{ video.time }}</p>
          <div class="textbox">
            <b-card-text>{{ video.title }} </b-card-text>
            <span>{{ video.user }}</span>
            <button>
              <img src="../assets/img/seealot.png" alt="" />
            </button>
          </div>
        </b-card>
 
    </div>
</template>
<script>
export default {
    props:["video","index","title","img","time","user"],
    name:"Video"
}
</script>