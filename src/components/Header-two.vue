<template>
  <div>
    <b-row class="m-0">
      <b-container class="p-0">
        <b-col md="11" class="mx-auto p-0">
          <b-navbar toggleable="lg" class="p-0">
            <b-navbar-brand href="#">
              <img
                src="../assets/images/logo1.jpg"
                alt="moviak"
                width="150px"
              />
            </b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
            <b-collapse id="nav-collapse" is-nav>
              <!-- Right aligned nav items -->
              <b-navbar-nav>
                <b-nav-form>
                  <b-form-input
                    size="sm"
                    class="mr-sm-2 navbar-input"
                    placeholder="Movie Search..."
                  ></b-form-input>
                  <button
                    type="button"
                    size="sm"
                    class="my-2 my-sm-0 roundBtn border-0"
                  >
                    GO
                  </button>
                </b-nav-form>
              </b-navbar-nav>
              <b-navbar-nav class="ml-auto mr-3">
                <b-nav-item href="#" class="ml-4">HOME</b-nav-item>
                <b-nav-item href="#" class="ml-4">MOVIE LAYOUT</b-nav-item>
                <b-nav-item href="#" class="ml-4">PAGE SINGLE</b-nav-item>
                <b-nav-item href="#" class="ml-4">SHOW TIME</b-nav-item>
                <b-nav-item href="#" class="ml-4">TOP RATED</b-nav-item>
              </b-navbar-nav>
            </b-collapse>
          </b-navbar>
        </b-col>
      </b-container>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "HeaderTwo"
};
</script>
<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css?family=Roboto+Condensed");
@import "../assets/scss/_variables.scss";

.navbar-input {
  border-radius: 20px;
  :focus {
    outline: none !important;
  }
}

.roundBtn {
  background-color: $darkOrange;
  outline: none;
  font-size: 11px;
  font-weight: 800;
  text-align: center;
  width: 30px;
  height: 30px;
  border-radius: 100%;
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
  text-decoration: none;
  &:hover {
    background-color: $darkOrange;
  }
  &:active {
    background-color: $darkOrange;
  }
}

.navbar-light .navbar-nav .nav-link {
  font-family: $robotoC;
  font-size: 12px;
  font-weight: 600;
  letter-spacing: 0.5px;
  color: #000;

  &:hover {
    color: #000;
    transition: 0.2s;
  }
}
.navbar-input {
  border: 2px solid #dfdfdf;

  &::placeholder {
    font-size: 12px;
    margin: 5px;
  }
}
</style>
