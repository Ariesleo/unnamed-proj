<template>
<div>
  <form>
    <div class="form-group">
      <textarea class="form-control" rows="27" id="comment"
      placeholder="START TRANSCRIBING HERE"></textarea>
    </div>
  </form>
</div>

</template>

<style scoped>
form {
  box-shadow: 5px 5px 15px rgba(119, 117, 117, 0.514);
  margin-top: 50px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 60%;
}
form:hover {
  transform: scale(1.01);
  box-shadow: 5px 5px 10px rgba(81, 61, 192, 0.651);
  transition: 0.3s;
}
textarea {
  font-size: 18px;
  font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI',
  Roboto, Oxygen, Ubuntu, Cantarell,
  'Open Sans', 'Helvetica Neue', sans-serif;
}

</style>
