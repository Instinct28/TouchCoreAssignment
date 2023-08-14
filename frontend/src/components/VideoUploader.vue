<template>
  <div>
    <input type="file" @change="uploadVideo" />
  </div>
</template>

<script>
export default {
  methods: {
    uploadVideo(event) {
      const file = event.target.files[0];
      // Use an API call to upload the file to the backend
    },
  },
};
</script>
