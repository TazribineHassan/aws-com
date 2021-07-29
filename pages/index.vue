<template>
  <section class="section-body">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-md-6 text-center mb-2">
          <h2 class="text-white font-weight-bold">AWS com</h2>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-md-7 col-lg-5">
          <div class="login-wrap p-4 p-md-5">
            <div
              class="
                icon
                d-flex
                align-items-center
                bg-blue
                justify-content-center
              "
            >
              <span class="fa fa-user text-white"></span>
            </div>
            <h3 class="text-center mb-4">Esapce admin</h3>
            <form class="login-form" method="post" action="@ViewBag.action">
              <div class="input-group mb-3">
                <div class="input-group-prepend">
                  <span
                    class="input-group-text bg-blue"
                    id="validationTooltipUsernamePrepend"
                  >
                    <i class="fa fa-user text-white"></i>
                  </span>
                </div>
                <input
                  type="email"
                  class="form-control border"
                  name="email"
                  placeholder="Email"
                />
              </div>
              <div class="input-group mb-4">
                <div class="input-group-prepend">
                  <span
                    class="input-group-text bg-blue"
                    id="validationTooltipUsernamePrepend"
                  >
                    <i class="fa fa-lock text-white"></i>
                  </span>
                </div>
                <input
                  type="password"
                  class="form-control border"
                  name="password"
                  placeholder="Mot de passe"
                />
              </div>
              <div class="form-group">
                <button
                  type="submit"
                  class="
                    form-control
                    btn
                    bg-blue
                    rounded
                    submit
                    px-3
                    text-white
                  "
                >
                  <i class="fas fa-sign-in-alt"></i> &nbsp;&nbsp; Connexion
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>


<style scoped>
.section-body {
    background-image: linear-gradient(-225deg, #83b0cc 0%, #3445b4 100%);
}
section {
    font-family: "Lato", Arial, sans-serif;
    font-size: 16px;
    line-height: 1.8;
    font-weight: normal;
    color: gray;
    height: -webkit-fill-available;
    /*background-image: linear-gradient(-225deg, #B7F8DB 0%, #50A7C2 100%);*/
    padding: 5em 0;
}

.bg-blue {
    background-color: #3445b4;
}

.login-wrap .icon {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    font-size: 30px;
    margin: 0 auto 10px;
}

.login-wrap {
    position: relative;
    background: #fff;
    border-radius: 10px;
    -moz-box-shadow: 0px 10px 34px -15px rgba(0, 0, 0, 0.24);
    box-shadow: -1px 1px 20px -10px rgba(0, 0, 0, 0.5);
}
</style>