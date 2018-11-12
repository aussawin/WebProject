<template>
    <div id = "thirty-years"></div>
</template>

<script>    
export default {

}
</script>

<style scoped>
#thirty-years {
    width: 100vw;
    height: 90vh;
    background-image: url("../assets/Image/2_30years/background.png");
    background-size: cover;
    background-repeat: no-repeat;
}
.grid-container {
  display: grid;
  grid-template-areas: 
    "area1 area2"
    "area1 area2";
  height: 100%;
  width: 80%;
}
.area1 { grid-area: area1; }
.area2 { grid-area: area2; }
.center {
    margin: auto;
}

.wrapper1 {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 20vh;
  grid-template-areas: 
    ". . . ."
    ". a a ."
    ". a a ."
    ". . . .";
}
.item1 {
  grid-area: a;
  align-self: center;
  justify-self: center;
}

</style>
