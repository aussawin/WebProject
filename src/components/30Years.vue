<template>
    <div id = "thirty-years">
        <div class="grid-container">
            <div class="area1">
                <div class="wrapper">
                    <div class="item1">
                        <img src="../assets/Image/2_30years/logo-30.png">
                    </div>
                </div>
            </div>
            <div class="area2 ">
                <center><h1><b>OF CONSTANT</b></h1></center>
            </div>
        </div>
    </div>
</template>

<script>    
export default {

}
</script>

<style scoped>
#thirty-years {
    width: 100vw;
    height: 80vh;
    background-image: url("../assets/Image/2_30years/BG.png");
    background-size: cover;
    background-repeat: no-repeat;
}
.grid-container {
  display: grid;
  grid-template-areas: 'area1 area2';
  height: 100%;
  width: 80%;
}
.area1 { grid-area: area1; }
.area2 { grid-area: area2; }
.center {
    margin: auto;
}

.wrapper {
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
