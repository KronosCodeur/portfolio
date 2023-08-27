<template>
  <div :style="viewerStyles" class="image-viewer">
    <div class="image-container">
      <img :src="imageSrc" alt="Image" class="full-image">
    </div>
    <div class="message-container">
      <div class="message-box d-flex align-center justify-center flex-row">
          <v-icon color="#01AF49" size="60" class="mr-1">fa-regular fa-circle-check</v-icon>
          <div class="d-flex align-start justify-center flex-column">
            <h3>+10</h3>
            <h4>{{ message }}</h4>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ImageViewer',
  props: {
    width: {
      type: String,
      default: '100%'
    },
    height: {
      type: String,
      default: '100vh'
    },
    imageSrc: {
      type: String,
      required: true
    },
    message: {
      type: String,
      default: 'Your message here'
    }
  },
  computed: {
    viewerStyles() {
      return {
        width: this.width,
        height: this.height
      };
    }
  }
};
</script>

<style scoped>
.image-viewer {
  position: relative;
  display: flex;
  border-radius: 40px 5px 5px 5px;
  align-items: center;
  justify-content: center;
}

.image-container {
  flex: 1;
  border-radius: 40px 5px 5px 5px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.full-image {
  width: 100%;
  border-radius: 40px 5px 5px 5px;
  height: 100%;
  object-fit: cover;
}

.message-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  padding-bottom: 30px;
  height: 100%;
  display: flex;
  align-items: end;
  justify-content: center;
  background-color: rgba(0, 0, 0, 0.1);
}

.message-box {
  color: white;
  text-align: start;
  width: 80%;
  height: 80px;
  border-radius: 25px;
  background: #0A0E11;
}
</style>
