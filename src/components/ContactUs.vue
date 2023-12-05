<template>
    <div>
    </div>
    <div class="contact-page  container-fluid">
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
      <div class="contactus-1 section-image" style="background-image: url('assets/img/contact1.jpg')">
            <div class="container">
              <div class="row">
                <div class="col-md-5">
                  <h2 class="title">Get in Touch</h2>
                  <h4 class="description">You need more information? Check what other persons are saying about our product. They are very happy with their purchase.</h4>
                  <div class="info info-horizontal">
                    <div class="icon icon-primary">
                      <i class="tim-icons icon-square-pin"></i>
                    </div>
                    <div class="description">
                      <h4 class="info-title">Find us at the office</h4>
                      <p class="description"> Bld Mihail Kogalniceanu, nr. 8,
                        <br> 7652 Bucharest,
                        <br> Romania
                      </p>
                    </div>
                  </div>
                  <div class="info info-horizontal">
                    <div class="icon icon-primary">
                      <i class="tim-icons icon-mobile"></i>
                    </div>
                    <div class="description">
                      <h4 class="info-title">Give us a ring</h4>
                      <p class="description"> Michael Jordan
                        <br> +40 762 321 762
                        <br> Mon - Fri, 8:00-22:00
                      </p>
                    </div>
                  </div>
                </div>
                <div class="col-md-5 ml-auto mr-auto">
                  <div class="card card-contact card-raised">
                    <form role="form" id="contact-form" method="post">
                      <div class="card-header text-center">
                        <h4 class="card-title">Contact Us</h4>
                      </div>
                      <div class="card-body">
                        <div class="row">
                          <div class="col-md-6">
                            <label>First name</label>
                            <div class="input-group">
                              <div class="input-group-prepend">
                                <span class="input-group-text"><i class="tim-icons icon-single-02"></i></span>
                              </div>
                              <input type="text" class="form-control" placeholder="First Name..." aria-label="First Name...">
                            </div>
                          </div>
                          <div class="col-md-6 pl-2">
                            <div class="form-group">
                              <label>Last name</label>
                              <div class="input-group">
                                <div class="input-group-prepend">
                                  <span class="input-group-text"><i class="tim-icons icon-caps-small"></i></span>
                                </div>
                                <input type="text" class="form-control" placeholder="Last Name..." aria-label="Last Name...">
                              </div>
                            </div>
                          </div>
                        </div>
                        <div class="form-group">
                          <label>Email address</label>
                          <div class="input-group">
                            <div class="input-group-prepend">
                              <span class="input-group-text"><i class="tim-icons icon-email-85"></i></span>
                            </div>
                            <input type="text" class="form-control" placeholder="Email Here...">
                          </div>
                        </div>
                        <div class="form-group">
                          <label>Your message</label>
                          <textarea name="message" class="form-control" id="message" rows="6"></textarea>
                        </div>
                        <div class="row">
                          <div class="col-md-6">
                            <div class="form-check">
                              <label class="form-check-label">
                                <input class="form-check-input" type="checkbox">
                                <span class="form-check-sign"></span>
                                I'm not a robot
                              </label>
                            </div>
                          </div>
                          <div class="col-md-6">
                            <button type="submit" class="btn btn-primary btn-round pull-right">Send Message</button>
                          </div>
                        </div>
                      </div>
                    </form>
                  </div>
                </div>
              </div>
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
