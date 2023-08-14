<template>
  <div>
    <video ref="videoRef" controls @timeupdate="syncSubtitles">
      <source :src="videoSrc" type="video/mp4" />
    </video>
    <div v-for="subtitle in subtitles" :key="subtitle.timestamp">
      {{ subtitle.text }}
    </div>
  </div>
</template>

<script>
export default {
  props: ['videoSrc', 'subtitles'],
  methods: {
    syncSubtitles(event) {
      // Update displayed subtitles based on the current video timestamp
    },
  },
};
</script>
