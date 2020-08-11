<template>
  <div class="container">
    <!--below is the floating window for youtube link-->
    <div id="floatwindow">
      <div class="form-group">
        <label for="inputEmail">Enter Youtube Video URL:</label
        ><button @click="closeWindow()" class="btncross">
          Cancle
          <i class="fas fa-times"></i>
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
    <button id="btnchose" type="button" class="btn btn-primary">
      <input type="file" accept="audio/*, video/*" name="" id="file" hidden />
      <label for="file" id="selector"
        ><i id="fontupload" class="fas fa-upload"></i><br />
        Choose audio(or video) file</label
      >
    </button>
    <br />
    <!--below button for youtube link button-->
    <button
      id="btnyou"
      @click="openWindow()"
      type="button"
      class="btn btn-primary"
      style="margin-top: 5px; width: 230px;"
    >
      Or YouTube Video
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
    openWindow() {
      const x = document.getElementById('floatwindow');
      // eslint-disable-next-line no-multi-assign
      const y = (x.style.display = 'block');
      return y;
    },
    closeWindow() {
      const x = document.getElementById('floatwindow');
      // eslint-disable-next-line no-multi-assign
      const y = (x.style.display = 'none');
      return y;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  margin-top: 20px;
}
#btnchose {
  width: 230px;
}
#btnchose:hover,
#btnyou:hover {
  transform: scale(1.08);
  box-shadow: 2px 2px 10px rgba(92, 91, 91, 0.89);
  transition: 0.5s ease;
}
/*below is the css for FLOATING WINDOW for youtube URL */
#floatwindow {
  color: aliceblue;
  margin-top: 10px;
  width: 400px;
  height: 88px;
  background-color: rgba(17, 16, 16, 0.897);
  border-radius: 5px;
  display: none;
  margin-left: auto;
  margin-right: auto;
  padding: 10px;
  margin-bottom: 10px;
}

.btncross {
  box-shadow: none !important;
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
