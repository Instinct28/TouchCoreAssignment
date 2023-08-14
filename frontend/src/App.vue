<template>
    <div id="app">
      <header>
        <h1>Video Subtitle App</h1>
      </header>
      <main>
        <!-- Your components go here -->
        <VideoUploader />
        <SubtitleEditor />
        <VideoPlayer :videoSrc="videoSrc" :subtitles="subtitles" />
      </main>
    </div>
  </template>
  
  <script>
  import VideoUploader from './components/VideoUploader.vue';
  import SubtitleEditor from './components/SubtitleEditor.vue';
  import VideoPlayer from './components/VideoPlayer.vue';
  
  export default {
    components: {
      VideoUploader,
      SubtitleEditor,
      VideoPlayer,
    },
    data() {
      return {
        videoSrc: 'path/to/your/video.mp4', // Update with your actual video path
        subtitles: [], // Array to hold subtitle data
      };
    },
  };
  </script>
  
  <style>
  /* Your styling goes here */
  </style>
  