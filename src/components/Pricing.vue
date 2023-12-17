<template>
  <div
    class="pricing-5"
    id="pricing-5"
  >
    <div class="space-50"></div>
    <div class="container">
      <div class="row">
        <div class="col-md-6 ml-auto mr-auto text-center">
          <h2 class="title text-white">Pick the best plan hosting plan for you</h2>
          <!-- <h4 class="description">You have Free Unlimited Updates and Premium Support on each package.</h4> -->
          <div class="section-space"></div>
        </div>
      </div>
      <div class="space-50"></div>
      <div class="row">
        <div class="col-md-4">
          <div class="card card-pricing card-plain card-primary">
            <div class="card-body">
              <h2 class="title">Shared Hosting</h2>
              <h5 class="description">
                $15
                <small>/Monthly</small>
              </h5>
              <ul>
                <li>Free SSL</li>
                <li>50GB Storage</li>
                <li>Unmetered Bandwidth</li>
                <li>Unlimited Hosted Domain</li>
                <li>Unlimited Email Accounts</li>
                <li>Free Drag & Drop Builder</li>
              </ul>
              <a
                class="btn btn-info btn-round contact-button"
                @click="$emit('scroll', 'Contact-us')"
              >
                Contact Us
              </a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card card-pricing card-plain card-primary">
            <div class="card-body">
              <h2 class="title">VPS Hosting</h2>
              <h5 class="description">
                $75
                <small>/Monthly</small>
              </h5>
              <ul>
                <li>Windows Server 2022</li>
                <li>vCPU : 6</li>
                <li>Physical RAM : 16 GB</li>
                <li>Unlimited Hosted Domain</li>
                <li>DISK SPACE : 400 GB SSD</li>
                <li>BANDWIDTH : 32 TB Out + Unlimited In</li>
              </ul>
              <a
                class="btn btn-info btn-round contact-button"
                @click="$emit('scroll', 'Contact-us')"
              >
                Contact Us
              </a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card card-pricing card-plain card-primary">
            <div class="card-body">
              <h2 class="title">
                Reseller Hosting
                <!-- <span class="badge badge-warning">Popular</span> -->
              </h2>
              <h5 class="description">
                $50
                <small>/Monthly</small>
              </h5>
              <ul>
                <li>Free SSL</li>
                <li>50 cPanel Accounts</li>
                <li>2GB Live RAM (per cpanel)</li>
                <li>24/7 Tech Support</li>
                <li>Unlimited Bandwidth</li>
                <li>Unlimited Email Accounts</li>
              </ul>
              <a
                class="btn btn-info btn-round contact-button"
                @click="$emit('scroll', 'Contact-us')"
              >
                Contact Us
              </a>
            </div>
          </div>
        </div>
        <!-- <div class="col-md-4">
          <div class="card card-pricing card-plain card-primary">
            <div class="card-body">
              <h2 class="title">Exclusive</h2>
              <h5 class="description">
                $13.99
                <small>/Monthly</small>
              </h5>
              <ul>
                <li>5 GB of space</li>
                <li>UnLimited Support</li>
                <li>Unlimited Downloads</li>
                <li>Full cloud access</li>
              </ul>
              <a
                href="javascript:;"
                class="btn btn-info btn-round"
              >
                Choose plan
              </a>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<style lang="scss">

.contact-button {
  color: white !important;
}

</style>
