<template>
  <section>
    <nav
      class="navbar navbar-expand-lg fixed-top navbar-transparent"
      color-on-scroll="300"
    >
      <div class="container">
        <div class="navbar-translate">
          <a
            class="navbar-brand"
            href="https://demos.creative-tim.com/blk-design-system-pro/index.html"
            rel="tooltip"
            title="Designed and Coded by Creative Tim"
            data-placement="bottom"
            target="_blank"
          >
          <img 
            src="../assets/img/digisol-white.png"
            style="height: 50px; width: fit-content;"
            />
            
          </a>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navigation"
            aria-controls="navigation-index"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-bar bar1"></span>
            <span class="navbar-toggler-bar bar2"></span>
            <span class="navbar-toggler-bar bar3"></span>
          </button>
        </div>
        <div
          class="collapse navbar-collapse"
          id="navigation"
        >
          <div class="navbar-collapse-header">
            <div class="row">
              <div class="col-6 collapse-brand">
                <a>
                  BLK•
                  <span> PRO </span>
                </a>
              </div>
              <div class="col-6 collapse-close text-right">
                <button
                  type="button"
                  class="navbar-toggler"
                  data-toggle="collapse"
                  data-target="#navigation"
                  aria-controls="navigation-index"
                  aria-expanded="false"
                  aria-label="Toggle navigation"
                >
                  <i class="tim-icons icon-simple-remove"></i>
                </button>
              </div>
            </div>
          </div>
          <ul class="navbar-nav ml-auto">
            <!-- <li class="dropdown nav-item">
              <a
                class="nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'PageHeader')"
              >
                <i class="tim-icons icon-paper"></i> PageHeader
              </a>
            </li> -->
            <li class="nav-item">
              <a
                class="dropdown nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'Features')"
              >
                <!-- <i class="tim-icons icon-paper"></i>  -->
                <span class="nav-text">Services</span>
              </a>
            </li>
            <!-- <li class="dropdown nav-item">
              <a
                class="nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'Services')"
              >
                <i class="tim-icons icon-paper"></i> Services
              </a>
            </li> -->
            <li class="dropdown nav-item">
              <a
                class="nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'Pricing')"
              >
                <!-- <i class="tim-icons icon-paper"></i>  -->
                <span class="nav-text">Pricing</span>
              </a>
            </li>
            <li class="dropdown nav-item">
              <a
                class="nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'Projects')"
              >
                <!-- <i class="tim-icons icon-paper"></i>  -->
                <span class="nav-text">Projects</span>
              </a>
            </li>
            <li class="dropdown nav-item">
              <a
                class="nav-link"
                data-toggle="dropdown"
                @click="$emit('scroll', 'Contact-us')"
              >
                <!-- <i class="tim-icons icon-paper"></i>  -->
                <span class="nav-text">Contact Us</span>
            </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </section>
</template>


<style lang="scss" scoped>

.nav-text {
  font-size: medium !important;
  font-weight: bold;
}

.nav-button {
  background-color: magenta ;
  border-radius: 3rem;
  box-shadow: none;
  border: none;
}
</style>
