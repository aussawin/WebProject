<template>
  <div id="society">
    <img src="../assets/Image/6_Society/Head.png">

    <div class="grid-container">
      <div class="activities-society"></div>

      <div class="csr-society"></div>

      <div class="safety-society"></div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Society",
  }

</script>

<style scoped>
  #society {
    width: 100vw;
    height: 70vh;
    padding-top: 5vh;
    padding-bottom: 10vh;
    padding-left: 15vw;
    padding-right: 15vw;
    background-color: rgb(252, 179, 53);
  }

  .grid-container {
    padding-top: 5vh;
    display: grid;
    grid-template-areas:
      'society1 society2 society3';
    grid-column-gap: 3vh;
  }

  .grid-container>div {
    height: 50vh;
    background-color: white;
  }

  .activities-society {
    grid-area: society1;
    background-image: url("../assets/Image/6_Society/Photo01.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .csr-society {
    grid-area: society2;
    background-image: url("../assets/Image/6_Society/Photo02.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .safety-society {
    grid-area: society3;
    background-image: url("../assets/Image/6_Society/Photo03.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

</style>
