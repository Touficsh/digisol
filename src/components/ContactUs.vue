<template>
  <div></div>
  <div class="contact-page container-fluid">
    <!-- <div class="row">
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
                <div class="col-md-6">
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
                </div>
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
      </div> -->
    <div
      class="contactus-1 section-image"
      style="background-image: url('assets/img/contact1.jpg')"
    >
      <div class="container">
        <div class="row">
          <div class="col-md-5">
            <h2 class="title">Get in Touch</h2>
            <!-- <h4 class="description">You need more information?</h4> -->
            <div class="info info-horizontal">
              <div class="icon icon-primary">
                <i class="tim-icons icon-square-pin"></i>
              </div>
              <div class="description">
                <h4 class="info-title">Find us at the office</h4>
                <p class="description">
                  Beirut Digital District, <br />
                  Beirut, <br />
                  Lebanon
                </p>
              </div>
            </div>
            <div class="info info-horizontal">
              <div class="icon icon-primary">
                <i class="tim-icons icon-mobile"></i>
              </div>
              <div class="description">
                <h4 class="info-title">Give us a ring</h4>
                <p class="description">
                  Saleh Halawani <br />
                  +961 71 565 742 <br />
                  Mon - Fri, 8:00-22:00
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-5 ml-auto mr-auto">
            <div class="card abc card-contact card-raised">
              <form
                role="form"
                class="p-3"
                id="contact-form"
                method="post"
                @submit.prevent="sendEmail"
              >
                <div class="card-header text-center">
                  <h4 class="card-title">Contact Us</h4>
                </div>
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
                          @blur="validateName"
                        />
                      </div>
                    </div>
                    <div class="col-md-12">
                      <div class="form-group">
                        <label>Phone number</label>
                        <div class="input-group">
                          <div class="input-group-prepend">
                            <span class="input-group-text"
                              ><i
                                class="fa fa-phone"
                                aria-hidden="true"
                              ></i
                            ></span>
                          </div>
                          <input
                            v-model.number="phone"
                            type="number"
                            name="phone"
                            id="phone"
                            class="form-control"
                            placeholder="Phone number"
                            aria-label="Phone number"
                          />
                        </div>
                      </div>
                    </div>
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
                    <div class="col-md-6">
                      <div class="form-check">
                        <!-- <label class="form-check-label">
                                <input class="form-check-input" type="checkbox">
                                <span class="form-check-sign"></span>
                                I'm not a robot
                              </label> -->
                      </div>
                    </div>
                  </div>
                  <div class="text-center mt-4">
                    <button
                      type="submit"
                      :disabled="!isFormValid()"
                      class="btn btn-primary btn-round"
                    >
                      Send Message
                    </button>
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
      phone: undefined,
      email: '',
      message: '',
    };
  },
  watch: {
    
  },
  methods: {
    validateName() {
      return this.from_name.trim() !== '';
    },
    validateEmail() {
      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return emailRegex.test(this.email);
    },
    validatePhone() {
      // Basic phone number pattern (customize as needed)
      const phoneRegex = /^\d{8,14}$/;
      return phoneRegex.test(this.phone);
    },
    validateMessage() {
      return this.message.trim() !== '';
    },
    isFormValid() {
      return (
        this.validateName() &&
        this.validateEmail() &&
        this.validatePhone() &&
        this.validateMessage()
      );
    },
    sendEmail(e) {
      if(this.isFormValid()) {
        try {
          emailjs.sendForm(
            'service_6yzhbpx',
            'template_63ig2d4',
            e.target,
            'IWUkJ0mEMybkb8zDa',
            {
              from_name: this.from_name,
              phone: this.phone,
              email: this.email,
              message: this.message,
            }
          );
        } catch (error) {
          console.log({ error });
        }
        // Reset form field
        this.from_name = '';
        this.phone = '';
        this.email = '';
        this.message = '';
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.abc {
  height: 540px;
}

.validation {
  color: magenta;
}
</style>
