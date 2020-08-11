<template>
  <!--Button import and Export STARTS here-->
  <div class="btnlst">
    <button class="sbutton-imp">
      <i id="icon-imp" class="fa fa-sign-in"></i>
      <span style="font-weight: lighter;">import</span></button
    ><br />

    <button class="sbutton-exp">
      <i id="icon-imp" class="fa fa-share-square-o"></i>
      <span>export</span>
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
  box-shadow: none !important;
  border: none;
  background-color: rgba(228, 225, 225, 0.911);
}
.sbutton-exp:hover,
.sbutton-imp:hover {
  transform: scale(1.2);
  box-shadow: 2px 2px 10px rgba(92, 91, 91, 0.89);
  transition: 0.5s ease;
}
#icon-imp {
  border: 1px solid rgba(97, 92, 92, 0.911);
  border-radius: 3px;
  width: 25px;
  height: 29px;
  padding-top: 5px;
  margin-top: 5px;
}
</style>
