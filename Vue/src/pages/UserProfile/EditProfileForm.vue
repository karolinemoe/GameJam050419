<template>
  <card class="card" title="Add content to PLED database">
    <div>
      <form @submit.prevent>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="Application Name"
                      placeholder="Application name">
            </fg-input>
          </div>

          
          <div class="col-md-7">
            <fg-input type="text"
                      label="CVE-ID (CVE-YYYY-XXXX)"
                      placeholder="CVE-ID">
            </fg-input>
          </div>
          
        </div>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="Application Summary"
                      placeholder="Application Summary">
            </fg-input>
          </div>

   
            <div class="col-md-7">
              <fg-input type="text"
                        label="CVSS"
                        placeholder="CVSS">
              </fg-input>
            </div>
      
        </div>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="File"
                      placeholder="file">
            </fg-input>
          </div>


          <div class="col-md-7">
            <fg-input type="text"
                      label="CVE Summary"
                      placeholder="CVE Summary">
            </fg-input>
          </div>
        </div>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="Category"
                      placeholder="Category">
            </fg-input>
          </div>
        </div>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="Platform"
                      placeholder="PLatform">
            </fg-input>
          </div>
        </div>

        <div class="row">
          <div class="col-md-5">
            <fg-input type="text"
                      label="Tag"
                      placeholder="Tag">
            </fg-input>
          </div>
        </div>

        <!--
        <div class="row">
          <div class="col-md-12">
            <div class="form-group">
              <label>About Me</label>
              <textarea rows="5" class="form-control border-input"
                        placeholder="Here can be your description"
                        v-model="user.aboutMe">

              </textarea>
            </div>
          </div>
        </div>
        -->


        <div class="text-center">
          <p-button block type="info"
                    round
                    @click.native.prevent="addContent">
            Add Content
          </p-button>
        </div>
        <div class="clearfix"></div>
      </form>
    </div>
  </card>
</template>
<script>
export default {
  data() {
    return {
      user: {
        company: "Paper Dashboard",
        username: "michael23",
        email: "",
        lastName: "Faker",
        address: "Melbourne, Australia",
        city: "melbourne",
        postalCode: "",
        aboutMe: `Oh so, your weak rhyme. You doubt I'll bother, reading into it.I'll probably won't, left to my own devicesBut that's the difference in our opinions.`
      }
    };
  },
  methods: {
    updateProfile() {
      alert("Your data: " + JSON.stringify(this.user));
    }
  }
};
</script>
<style>
</style>
