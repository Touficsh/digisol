<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="title abc">
            <img
              src="../assets/img/digisol-white.png"
              style="height: 50px; width: fit-content"
            />
          </div>
        </div>
        <div class="col-md-6 title abc">
          <!-- <span class="footer_wording">Follow us:</span> -->
          <div class="col-md-6 col-sm-6">
                <button class="btn btn-dribbble">
                  <i class="fab fa-instagram"></i> Follow us on Instagram
                </button>
              </div>
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

.abc {
  text-align: center !important;
}
</style>
