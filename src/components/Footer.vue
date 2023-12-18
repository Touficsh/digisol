<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="title abc">
            <img
              src="../assets/img/digisol-white.png"
              style="height: 30px; width: 100px;"
            />
          </div>
        </div>
        <div class="col-md-6 title abc">
          <!-- <span class="footer_wording">Follow us:</span> -->
          <div class="col-md-6 col-sm-6">
                <a class="btn btn-instagram"
                href="https://www.instagram.com/digisol.innovations?igshid=YTQwZjQ0NmI0OA=="
                >
                  <i class="fab fa-instagram"></i> Follow us on Instagram
                </a>
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
