<template>
      <div class="goto-container mt-5" data-bs-toggle="tooltip" data-bs-placement="top" title="Go to top">
    <button id="topbtn" class="gotop"><i class="display-4 bi bi-arrow-up"></i></button>
  </div>
</template>

<script>
export default{
    name: 'go-to-top'
}

</script>

<style>

.goto-container {
  width: 50px;
  margin-left: 90%;
}
.gotop {
  display: inline-block;
  position: fixed;
  z-index: 99;
  background-color: black;
  color: rgb(231, 218, 218);
  border-radius: 100%;
  outline: none;
  padding-bottom: 0.35ch;
  border: 4px;
  /* transition: all 600ms cubic-bezier(.23, 1, 0.32, 1); */
  text-decoration: none;
  box-shadow: rgba(0, 0, 0, 0.25) 0 2px 5px;
  opacity: 0.85;

}

.gotop:hover{
    cursor: pointer;
    border: 1px solid black;
    color: black;
    transform: translateY(-10px);
    transition: all 200ms cubic-bezier(.23, 1, 0.32, 1);
    background-color: #ffffff;
  }

@media only screen and (max-width: 576px) {
.goto-container {
  margin-left: 85%;
}
}

</style>