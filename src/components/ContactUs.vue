<template>
    <div 
    class="contact-us">
      <div
        class="page-header-image"
        style="background-image: url('../assets/img/andre-benz.jpg')"
      ></div>
      <div class="container">
        <div class="row">
          <div class="col-md-12 text-center">
            <h1 class="title">Got a question?</h1>
            <h3>We'd like to talk more about what you need</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="contact-page  container-fluid">
      <div class="row infos mb-5">
        <div class="col-lg-3">
          <div class="info info-hover">
            <div class="icon icon-primary">
              <img
                class="bg-blob"
                src="../assets/img/feature-blob/primary.png"
              />
              <i class="tim-icons icon-square-pin"></i>
            </div>
            <h4 class="info-title">Address</h4>
            <p class="description">12124 First Street, nr 54</p>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="info info-hover">
            <div class="icon icon-info">
              <img
                class="bg-blob"
                src="../assets/img/feature-blob/info.png"
              />
              <i class="tim-icons icon-email-85"></i>
            </div>
            <h4 class="info-title">Email</h4>
            <p class="description">support@youremail.com</p>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="info info-hover">
            <div class="icon icon-warning">
              <img
                class="bg-blob"
                src="../assets/img/feature-blob/warning.png"
              />
              <i class="tim-icons icon-mobile"></i>
            </div>
            <h4 class="info-title">Phone Number</h4>
            <p class="description">+1(424) 535 3523</p>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="info info-hover">
            <div class="icon icon-success">
              <img
                class="bg-blob"
                src="../assets/img/feature-blob/success.png"
              />
              <i class="tim-icons icon-single-02"></i>
            </div>
            <h4 class="info-title">Contact</h4>
            <p class="description">Andrew Samian</p>
          </div>
        </div>
      </div>
      <div class="row mt-5 mb-4 pt-5">
        <div class="col-md-8 ml-auto mr-auto text-center mt-5">
          <span class="badge badge-info">Leave a message</span>
          <h1 class="title">
            Tell us more about
            <b>yourself</b>
          </h1>
          <h4 class="desc">
            Whether you have questions or you would just like to say hello,
            contact us.
          </h4>
        </div>
      </div>
      <div class="row">
        <div class="col-md-10 mx-auto">
          <form
            role="form"
            class="p-3"
            id="contact-form"
            method="post"
            @submit.prevent="sendEmail"
          >
            <div class="card-body">
              <div class="row">
                <div class="col-md-12">
                  <label>Full Name</label>
                  <div class="input-group">
                    <div class="input-group-prepend">
                      <span class="input-group-text"
                        ><i class="tim-icons icon-single-02"></i
                      ></span>
                    </div>
                    <input
                      v-model="from_name"
                      type="text"
                      name="from_name"
                      id="from_name"
                      class="form-control"
                      placeholder="Full Name"
                      aria-label="First Name..."
                    />
                  </div>
                </div>
                <!-- <div class="col-md-6">
                  <div class="form-group">
                    <label>Last name</label>
                    <div class="input-group">
                      <div class="input-group-prepend">
                        <span class="input-group-text"
                          ><i class="tim-icons icon-caps-small"></i
                        ></span>
                      </div>
                      <input
                        v-model="lastName"
                        type="text"
                        name="lastName"
                        id="lastName"
                        class="form-control"
                        placeholder="Last Name..."
                        aria-label="Last Name..."
                      />
                    </div>
                  </div>
                </div> -->
              </div>
              <div class="form-group">
                <label>Email address</label>
                <div class="input-group">
                  <div class="input-group-prepend">
                    <span class="input-group-text"
                      ><i class="tim-icons icon-email-85"></i
                    ></span>
                  </div>
                  <input
                    v-model="email"
                    type="text"
                    name="email"
                    id="email"
                    class="form-control"
                    placeholder="Email Address"
                  />
                </div>
              </div>
              <div class="form-group">
                <label>Your message</label>
                <textarea
                  v-model="message"
                  name="message"
                  class="form-control"
                  id="message"
                  rows="6"
                ></textarea>
              </div>
              <div class="row">
                <div class="col-md-6 ml-auto">
                  <button
                    type="submit"
                    class="btn btn-primary btn-round pull-right"
                  >
                    Send Message
                  </button>
                </div>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
</template>

<script>
import emailjs from 'emailjs-com';

export default {
  data() {
    return {
      from_name: '',
      email: '',
      message: ''
    }
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm('service_6yzhbpx', 'template_63ig2d4', e.target, 'IWUkJ0mEMybkb8zDa', {
          from_name: this.from_name,
          email: this.email,
          message: this.message
        })

      } catch(error) {
          console.log({error})
      }
      // Reset form field
      this.from_name = ''
      this.email = ''
      this.message = ''
    },
  }
}

</script>

<style scoped>
.contact-us {
  height: 200px;
}
</style>
