<template>
  <div id="contact-us">
    <img src="../assets/Image/8_Contact/Head.jpg">

    <div class="company-name">
      <p>PSP Specialties Co., Ltd.</p>
    </div>

    <div class="grid-container">
      <div class="bangkok-location">
        <h6><strong style="color: rgb(230, 231, 232);">Bangkok</strong></h6>
        <p>1 Boromrachachonanee Rd.</p>
        <p>Arun-Amarin. Bangkoknoi.</p>
        <p>Bangkok. 10700. Thailand.</p>
        <p>Telephone +662 4340540</p>
        <p>Fax +662 4336016</p>
        <p>Email: info@psp.co.th</p>
      </div>

      <div class="sales-contact">
        <h6><strong style="color: rgb(252, 179, 53);">Local sales</strong></h6>
        <p>+662 4336012-15 #3121</p> <br>
        <h6><strong style="color: rgb(252, 179, 53);">Export sales</strong></h6>
        <p>+662 4336012-15 #3116. #3126</p>
      </div>

      <div class="samutsakorn-loc1">
        <h6><strong style="color: rgb(230, 231, 232);">Samutsakorn Terminal 1</strong></h6>
        <p>76 Moo 7 T.Thachin.</p>
        <p>A.Muang Samutsakorn.</p>
        <p>74000 Thailand</p>
        <p>Telephone +6634 818671</p>
        <p>Fax +6634 819122</p>
      </div>

      <div class="samutsakorn-loc2">
        <h6><strong style="color: rgb(230, 231, 232);">Samutsakorn Terminal 2</strong></h6>
        <p>100/149 Moo 1 T.Thachin.</p>
        <p>A.Muang Samutsakorn</p>
        <p>74000 Thailand</p>
        <p>Telephone +6634 820519</p>
        <p>Fax +6634 820971</p>
      </div>

      <div class="form-input">
        <b-container fluid>
          <b-row class="my-1">
            <b-col sm="12">
              <b-form-input id="input-small" size="sm" type="text" placeholder="Your Name (required)" v-model="form.name"></b-form-input>
            </b-col>
          </b-row>
          <b-row class="my-1">
            <b-col sm="12">
              <b-form-input id="input-small" size="sm" type="text" placeholder="Your Email (required)" v-model="form.email"></b-form-input>
            </b-col>
          </b-row>
          <b-row class="my-1">
            <b-col sm="12">
              <b-form-input id="input-small" size="sm" type="text" placeholder="Subject" v-model="form.subject"></b-form-input>
            </b-col>
          </b-row>
          <b-row class="my-1">
            <b-col sm="12">
              <b-form-textarea id="textarea" placeholder="Your Message" :rows="5" :max-rows="6" v-model="form.message">
              </b-form-textarea>
            </b-col>
          </b-row>
          <b-row class="my-1">
            <b-col sm="4">
              <h1>Capcha</h1>
            </b-col>
            <b-col sm="8">
              <b-button :class="{disabled: btnState}" id="submit-btn" @click="submit">Submit</b-button>
            </b-col>
          </b-row>
        </b-container>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "ContactUs",
    data() {
        return {
            state: null,
            form: {
                name: '',
                email: '',
                subject: '',
                message: '',
            },
        }
    },
    methods: {
        submit: function() {

        },
    },
    computed: {
        btnState: function() {
            if (this.form.name.length == 0 || this.form.email.length == 0) {
                return true
            }
            
            return false
        },
    }
  }

</script>

<style scoped>
  #contact-us {
    width: 100vw;
    height: 65vh;
    padding-top: 10vh;
    padding-bottom: 10vh;
    padding-left: 15vw;
    padding-right: 15vw;
    background-color: rgb(65, 64, 66);
  }

  .grid-container {
    padding-top: 4vh;
    display: grid;
    grid-template-areas:
      'loc1 loc2 form form form form'
      'loc3 loc4 form form form form';
    grid-row-gap: 5vh;
  }

  p {
    margin: 0px;
    color: rgb(230, 231, 232);
  }

  .company-name {
    padding-top: 4vh;
    font-size: 28px;
    color: rgb(230, 231, 232);
  }

  .bangkok-location {
    grid-area: loc1;
    font-size: 14px;
  }

  .sales-contact {
    grid-area: loc2;
    font-size: 14px;
  }

  .samutsakorn-loc1 {
    grid-area: loc3;
    font-size: 14px;
  }

  .samutsakorn-loc2 {
    grid-area: loc4;
    font-size: 14px;
  }

  .form-input {
    grid-area: form;
    width: 100%;
  }

  #submit-btn {
    background-color: rgb(252, 179, 53);
    color: black;
    width: 100%;
  }

  .row {
    padding-bottom: 1.2vh;
  }

</style>
