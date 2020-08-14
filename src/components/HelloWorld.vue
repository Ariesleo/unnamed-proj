<template>
  <div class="container">
    <!--below is the floating window for youtube link-->
    <div class="floatwindow" ref="floatWindow" v-if="isFloatWindowOpen">
      <div class="form-group">
        <label for="inputEmail">Enter Youtube Video URL:</label
        ><button @click="closeWindow" class="btncross">
          Cancel
          <fa-icon class="fa" :icon="['fas', 'times']" />
        </button>
        <input
          type="email"
          class="form-control"
          id="inputEmail"
          placeholder="paste your link here"
        />
      </div>
    </div>
    <!--floating window ends here-->
    <button type="button" class="btn btn-primary">
      <input type="file" accept="audio/*, video/*" name="" id="file" hidden />
      <label for="file" id="selector"
        ><i id="fontupload" class="fas fa-upload"></i>
        <fa-icon class="fa" :icon="['fas', 'upload']" /><br />
        Choose audio(or video) file</label
      >
    </button>
    <br />
    <!--below button for youtube link button-->
    <button
      @click="openWindow"
      type="button"
      class="btn btn-primary"
    >
      Or YouTube Video
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      isFloatWindowOpen: false,
    };
  },
  methods: {
    openWindow() {
      this.isFloatWindowOpen = true;
    },
    closeWindow() {
      this.isFloatWindowOpen = false;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  margin-top: 20px;
}
.btn {
  width: 230px;
  margin-top: 5px;
  width: 230px;
}
.btn:hover {
  transform: scale(1.08);
  box-shadow: 2px 2px 10px rgba(92, 91, 91, 0.89);
  transition: 0.5s ease;
}
/*below is the css for FLOATING WINDOW for youtube URL */
.floatwindow {
  color: aliceblue;
  margin-top: 10px;
  width: 400px;
  height: 88px;
  background-color: rgba(17, 16, 16, 0.897);
  border-radius: 5px;
  margin-left: auto;
  margin-right: auto;
  padding: 10px;
  margin-bottom: 10px;
}

.btncross {
  border: none;
  background-color: rgba(46, 44, 44, 0.411);
  color: rgba(143, 146, 148, 0.521);
  float: right;
}
.btncross:hover {
  color: aliceblue;
}
/*FLOATING WINDOW ends HERE */
</style>
