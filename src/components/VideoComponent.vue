<template>
  <div v-if="videoSource == 1" class="custom-frame ma-6" @click="togglePlay">
    <video ref="videoElement" class="video-element">
      <source src="../assets/video/bitiruvchilar-1.mp4" type="video/mp4">
    </video>
    <v-btn density="comfortable" id="play-button" :icon="isPlaying ? ' mdi-play' : 'mdi-pause'"
      @click="isPlaying = !isPlaying" color="#B5976E"></v-btn>
    <div id="text-div">
      <p class="title">{{ title }}</p>
      <p class="title title2">{{ title2 }}</p>
      <h4 class="subtitles">{{ subtitles }}</h4>
    </div>

    <div @click="isPlaying = !isPlaying" id="black-bg"></div>
  </div>

  <div v-if="videoSource == 2" class="custom-frame ma-6" @click="togglePlay">
    <video ref="videoElement" class="video-element">
      <source src="../assets/video/bitiruvchilar-2.mp4" type="video/mp4">
    </video>
    <v-btn density="comfortable" id="play-button" :icon="isPlaying ? ' mdi-play' : 'mdi-pause'"
      @click="isPlaying = !isPlaying" color="#B5976E"></v-btn>
    <div id="text-div">
      <p class="title">{{ title }}</p>
      <p class="title title2">{{ title2 }}</p>
      <h4 class="subtitles">{{ subtitles }}</h4>
    </div>

    <div @click="isPlaying = !isPlaying" id="black-bg"></div>
  </div>

  <div v-if="videoSource == 3" class="custom-frame ma-6" @click="togglePlay">
    <video ref="videoElement" class="video-element">
      <source src="../assets/video/bitiruvchilar-3.mp4" type="video/mp4">
    </video>
    <v-btn density="comfortable" id="play-button" :icon="isPlaying ? ' mdi-play' : 'mdi-pause'"
      @click="isPlaying = !isPlaying" color="#B5976E"></v-btn>
    <div id="text-div">
      <p class="title">{{ title }}</p>
      <p class="title title2">{{ title2 }}</p>
      <h4 class="subtitles">{{ subtitles }}</h4>
    </div>

    <div @click="isPlaying = !isPlaying" id="black-bg"></div>
  </div>

  <div v-if="videoSource == 4" class="custom-frame ma-6" @click="togglePlay">
    <video ref="videoElement" class="video-element">
      <source src="../assets/video/bitiruvchilar-4.mp4" type="video/mp4">
    </video>
    <v-btn density="comfortable" id="play-button" :icon="isPlaying ? ' mdi-play' : 'mdi-pause'"
      @click="isPlaying = !isPlaying" color="#B5976E"></v-btn>
    <div id="text-div">
      <p class="title">{{ title }}</p>
      <p class="title title2">{{ title2 }}</p>
      <h4 class="subtitles">{{ subtitles }}</h4>
    </div>

    <div @click="isPlaying = !isPlaying" id="black-bg"></div>
  </div>


</template>

<script>
export default {
  data() {
    return {
      isPlaying: true,
    };
  },
  props: {
    videoSource: Number,
    title: String,
    title2: String,
    subtitles: String
  },
  methods: {
    togglePlay() {
      const video = this.$refs.videoElement;
      if (this.isPlaying) {
        video.pause();
      } else {
        video.play();
      }
    },
  },
};
</script>

<style scoped>
.custom-frame {
  padding: 0;
  height: 415px;
  width: 224px;
  position: relative;
  overflow: hidden;
}

.video-element {
  border-radius: 30px;
  padding: 0;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
}

#play-button {
  position: absolute;
  top: 20px;
  left: 20px;
  z-index: 10;
}

#text-div {
  color: white;
  position: absolute;
  bottom: 20px;
  left: 20px;
}

.title2 {
  color: #75C5A2;
}

#black-bg{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;  
}
</style>