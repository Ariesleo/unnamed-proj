<template>
  <!--Button import and Export STARTS here-->
  <div class="btnlst">
    <button class="sbutton-imp">
      <fa-icon class="fa" :icon="['fas', 'sign-in-alt']" />
        <span> Import</span></button
    ><br />

    <button class="sbutton-exp">
      <fa-icon class="fa" :icon="['fas', 'share-square']" />
      <span> Export</span>
    </button>
  </div>
  <!--Button import and Export ENDS here-->
</template>

<style scoped>
/*IMPORT EXPORT icon part */
.btnlst {
  position: fixed;
  margin-top: 10%;
  left: 85%;
}
.sbutton-imp,
.sbutton-exp {
  box-shadow: none;
  border: none;
  border-radius: 5px;
  background-color: white;
}
.sbutton-exp:hover,
.sbutton-imp:hover {
  transform: scale(1.2);
  box-shadow: 5px 5px 10px rgba(92, 91, 91, 0.89);
  transition: 0.5s ease;
}
.fa {
  border: 1px solid rgba(97, 92, 92, 0.911);
  border-radius: 3px;
  width: 25px;
  height: 29px;
  margin-top: 5px;
  margin-bottom: 0px;
  color: rgba(0, 0, 0, 0.89);
  font-size: 20px;
}
</style>
