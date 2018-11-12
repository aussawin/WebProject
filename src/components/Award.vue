<template>
  <div id="award">
    <img src="../assets/Image/7_Award/Head.png">

    <div class="grid-container">
      <div class="duns-award" @click="dunsAward"></div>

      <div class="bsi-award1" @click="bsi1Award"></div>

      <div class="bsi-award2" @click="bsi2Award"></div>

      <div class="ilac-award" @click="ilacAward"></div>
    </div>

    <modal name="duns-modal" height="auto">
      <slot name="body">
        <section class="modal-body">
          <img src="../assets/Image/7_Award/Award01/D-U-N-S-Certificated-PSP-Sep2017-2018.jpg">
        </section>
      </slot>
    </modal>

    <modal name="bsi1-modal" height="auto">
      <slot name="body">
        <section class="modal-body">
          <b-carousel style="text-shadow: 1px 1px 2px #333;" controls indicators background="#ababab" :interval="4000"
            img-width="1024" img-height="480">
            <b-carousel-slide img-src="../assets/Image/7_Award/Award02/01.jpg"></b-carousel-slide>
            <b-carousel-slide img-src="../assets/Image/7_Award/Award02/02.jpg"></b-carousel-slide>
          </b-carousel>
        </section>
      </slot>
    </modal>

    <modal name="bsi2-modal" height="auto">
      <slot name="body">
        <section class="modal-body">
          <b-carousel style="text-shadow: 1px 1px 2px #333;" controls indicators background="#ababab" :interval="4000"
            img-width="1024" img-height="480">
            <b-carousel-slide img-src="../assets/Image/7_Award/Award03/01.jpg"></b-carousel-slide>
            <b-carousel-slide img-src="../assets/Image/7_Award/Award03/02.jpg"></b-carousel-slide>
          </b-carousel>
        </section>
      </slot>
    </modal>

    <modal name="ilac-modal" height="auto">
      <slot name="body">
        <section class="modal-body">
          <b-carousel style="text-shadow: 1px 1px 2px #333;" controls indicators background="#ababab" :interval="4000"
            img-width="1024" img-height="480">
            <b-carousel-slide img-src="../assets/Image/7_Award/Award04/01.jpg"></b-carousel-slide>
            <b-carousel-slide img-src="../assets/Image/7_Award/Award04/02.jpg"></b-carousel-slide>
          </b-carousel>
        </section>
      </slot>
    </modal>
  </div>
</template>

<script>
  export default {
    name: "Award",
    methods: {
      dunsAward: function () {
        this.$modal.show("duns-modal")
      },
      bsi1Award: function() {
        this.$modal.show("bsi1-modal")
      },
      bsi2Award: function() {
        this.$modal.show("bsi2-modal")
      },
      ilacAward: function() {
        this.$modal.show("ilac-modal")
      }
    },
    mounted() {}
  }

</script>

<style scoped>
  #award {
    width: 100vw;
    height: 70vh;
    padding-top: 5vh;
    padding-bottom: 10vh;
    padding-left: 15vw;
    padding-right: 15vw;
    background-color: rgb(230, 231, 232);
  }

  .grid-container {
    padding-top: 5vh;
    display: grid;
    grid-template-areas:
      'award1 award2 award3 award4';
    grid-column-gap: 3vh;
  }

  .grid-container>div {
    height: 50vh;
    background-color: white;
  }

  .duns-award {
    grid-area: award1;
    background-image: url("../assets/Image/7_Award/Photo01.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .bsi-award1 {
    grid-area: award2;
    background-image: url("../assets/Image/7_Award/Photo02.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .bsi-award2 {
    grid-area: award3;
    background-image: url("../assets/Image/7_Award/Photo03.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .ilac-award {
    grid-area: award4;
    background-image: url("../assets/Image/7_Award/Photo04.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .modal-body {
    text-align: center;
  }

  .v--modal-box, .v--modal {
    background-color: red;
  }

</style>
