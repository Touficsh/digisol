<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="col-md-9">
          <div class="title">
            <img
              src="../assets/img/digisol-white.png"
              style="height: 50px; width: fit-content"
            />
          </div>
        </div>
        <div class="col-md-3 btn-wrapper profile text-center footer_icons">
          <span class="footer_wording">Follow us:</span>
          <a
            target="_blank"
            href="https://twitter.com/creativetim"
            class="btn btn-icon btn-neutral btn-round btn-simple"
            data-toggle="tooltip"
            data-original-title="Follow us"
          >
            <i class="fab fa-twitter"></i>
          </a>
          <a
            target="_blank"
            href="https://www.facebook.com/creativetim"
            class="btn btn-icon btn-neutral btn-round btn-simple"
            data-toggle="tooltip"
            data-original-title="Like us"
          >
            <i class="fab fa-facebook-square"></i>
          </a>
          <a
            target="_blank"
            href="https://dribbble.com/creativetim"
            class="btn btn-icon btn-neutral btn-round btn-simple"
            data-toggle="tooltip"
            data-original-title="Follow us"
          >
            <i class="fab fa-dribbble"></i>
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  padding-top: 0px !important;

  &_icons {
    display: flex;
    align-items: center; 
    align-content: center; 
  }

  &_wording {
    color: white;
    font-weight: bolder;
    font-size: large;
    margin-right: 20px;
  }
}
</style>
