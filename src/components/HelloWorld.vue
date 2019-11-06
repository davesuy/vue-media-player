<template>

  <div class="hello">

   <!-- audio element -->
     <div class="audio-con">
<vue-plyr>

  <audio>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3"/>
   
  </audio>

</vue-plyr>

 <vue-plyr ref="plyr"></vue-plyr>
     
     </div>
       
   
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  mounted() {
     console.log(this.player)
  },
  computed: {
    player () { return this.$refs.plyr.player }
  }
}
</script>

<style>
  .audio-con {
    max-width: 400px;
    margin: 0 auto;
    text-align: center;
    margin-top: 100px;
  }

  .audio-con .plyr__controls>.plyr__control:first-child {
    margin: 0;
  }
</style>






