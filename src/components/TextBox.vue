<template>
  <div class="textarea">
    <div class="mousetrap" contenteditable="true">
      <br /><br />
      <p></p>
    </div>
  </div>
</template>

<style scoped>
.textarea {
  background-color: white;
  padding: 50px;
  box-shadow: 5px 5px 15px rgba(119, 117, 117, 0.514);
  margin-top: 50px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 60%;
}
.textarea:hover {
  transform: scale(1.01);
  box-shadow: 2px 2px 10px rgba(92, 91, 91, 0.89);
  transition: 0.5s ease-in;
}
.mousetrap {
  text-align: start;
}
</style>
