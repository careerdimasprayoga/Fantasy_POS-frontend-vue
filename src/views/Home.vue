<template>
  <div class="d-flex" id="wrapper">
    <!-- Sidemenu -->
    <div class="sidemenu-box" id="sidemenu-wrapper">
      <b-row
        class="sidemenu-header-box text-center align-items-center"
        style="border-bottom: #cecece 1px solid;"
      >
        <b-col xl="12">
          <a href class="modify-link-text">Menu</a>
        </b-col>
      </b-row>
      <b-row class="sidemenu-header-box text-center align-items-center">
        <b-col xl="12">
          <a href class="modify-link-text">
            <img src="../assets/images/icons/fork.png" style="width: 40px; height: 40px;" />
          </a>
        </b-col>
      </b-row>
      <b-row class="sidemenu-header-box text-center align-items-center">
        <b-col xl="12">
          <a href class="modify-link-text">
            <img src="../assets/images/icons/clipboard.png" style="width: 40px; height: 40px;" />
          </a>
        </b-col>
      </b-row>
      <b-row class="sidemenu-header-box text-center align-items-center">
        <b-col xl="12">
          <a href class="modify-link-text">
            <img src="../assets/images/icons/add.png" style="width: 40px; height: 40px;" />
          </a>
        </b-col>
      </b-row>
    </div>
    <!-- End sidemenu -->

    <div id="page-content-wrapper">
      <b-container fluid>
        <!-- Header -->
        <b-row style="margin-left:0px;">
          <b-col xl="8" md="7" sm="7" xs="12" class="navbarOne">
            <b-container>
              <b-row>
                <b-col xl="1" lg="2" md="2" sm="2" class="col-2" style="margin-top: 15px;">
                  <button class="btn-custom" id="menu-toggle">
                    <img src="../assets/images/icons/menu.png" style="width: 30px; height: 30px" />
                  </button>
                </b-col>
                <b-col
                  xl="10"
                  lg="8"
                  md="8"
                  sm="8"
                  class="col-8 text-center"
                  style="margin-top: 5px;"
                >
                  <p style="font-size: 30px">Food Items</p>
                </b-col>
                <b-col xl="1" lg="2" md="2" sm="2" xs="1" class="col-2" style="margin-top: 15px;">
                  <button class="btn-custom">
                    <img src="../assets/images/icons/find.png" style="width: 30px; height: 30px" />
                  </button>
                </b-col>
              </b-row>
            </b-container>
          </b-col>
          <b-col xl="4" md="5" sm="5" class="navbarTwo text-center">
            <div class="d-flex justify-content-center">
              <p style="font-size: 30px; margin-top: 5px">Cart</p>
              <div
                class="cart-qty"
                style="width: 30px; height: 30px; background-color: #57CAD5; border-radius: 50px; margin-top: 15px; margin-left:5px;"
              >
                <p style="font-size: 25px; margin-top: -5px;color:white;">0</p>
              </div>
            </div>
          </b-col>
        </b-row>

        <!-- End Header -->
        <!-- Content -->
        <b-row style="margin-left:0px;">
          <b-col xl="12" md="12" sm="12" class="background-content">
            <!-- Food Items -->
            <b-row>
              <b-col
                xl="8"
                md="7"
                sm="7"
                style="padding-right: 30px;padding-left: 30px;padding-top: 20px;"
              >
                <b-container fluid>
                  <b-row>
                    <b-col xl="4" lg="6" md="12">
                      <b-card
                        v-bind:img-src="require('../assets/images/products/cappucino.jpg')"
                        img-alt="Image"
                        img-top
                        class="custom-card"
                      >
                        <b-card-text class="custom-card-text-name font-book">Espresso</b-card-text>
                        <b-card-text class="custom-card-text-price font-medium">Rp. 25.000</b-card-text>
                      </b-card>
                    </b-col>
                    <b-col xl="4" lg="6" md="12">
                      <b-card
                        v-bind:img-src="require('../assets/images/products/chocho_rum.jpg')"
                        img-alt="Image"
                        img-top
                        class="custom-card"
                      >
                        <b-card-text class="custom-card-text-name font-book">Choco Rhum</b-card-text>
                        <b-card-text class="custom-card-text-price font-medium">Rp. 35.000</b-card-text>
                      </b-card>
                    </b-col>
                    <b-col xl="4" lg="6" md="12">
                      <b-card
                        img-src="https://picsum.photos/300/220/?image=41"
                        img-alt="Image"
                        img-top
                        class="custom-card"
                      >
                        <b-card-text class="custom-card-text-name font-book">Cappucino</b-card-text>
                        <b-card-text class="custom-card-text-price font-medium">Rp. 5.000</b-card-text>
                      </b-card>
                    </b-col>
                    <b-col xl="4" lg="6" md="12">
                      <b-card
                        img-src="https://picsum.photos/300/220/?image=41"
                        img-alt="Image"
                        img-top
                        class="custom-card"
                      >
                        <b-card-text class="custom-card-text-name font-book">Red Velvet Latte</b-card-text>
                        <b-card-text class="custom-card-text-price font-medium">Rp. 35.000</b-card-text>
                      </b-card>
                    </b-col>
                  </b-row>
                </b-container>
              </b-col>
              <!-- End Food Items -->
              <!-- Cart -->
              <b-col xl="4" md="5" sm="5" xs="12" style="background-color: white;">
                <b-row>
                  <b-col xl="12">
                    <div class="text-center">
                      <img
                        src="../assets/images/icons/food_sidebar.png"
                        style="width: 250px; margin-top: 50px;"
                        class="col-12"
                        md="12"
                        sm="12"
                        xs="12"
                      />
                      <p
                        style="font-size: 25px; font-weight: bold; line-height: 10pt; margin-top: -20px;"
                      >Your cart is empty</p>
                      <p
                        style="font-size: 15px; font-weight: bold;color: #CECECE;"
                      >Please add some items from the menu</p>
                    </div>
                  </b-col>
                </b-row>
              </b-col>
              <!-- End Cart -->
            </b-row>
          </b-col>
        </b-row>
        <footer style="background-color: white;">
          <b-row>
            <b-col xl="12" class="footers text-center">
              <p style="margin-top: 10px;">Built with love by Dimas Prayoga</p>
            </b-col>
          </b-row>
        </footer>
        <!-- End Content -->
      </b-container>
    </div>
    <!-- end wrapper -->
  </div>
  <!-- end flex -->
</template>

<style scoped>
/* Global */
@font-face {
  font-family: 'AirbnbMedium';
  src: url('../assets/fonts/AirbnbCerealMedium.ttf');
}
@font-face {
  font-family: 'AirbnbBook';
  src: url('../assets/fonts/AirbnbCerealBook.ttf');
}
.font-medium {
  font-family: AirbnbMedium;
}
.font-book {
  font-family: AirbnbBook;
}
/* Modify Bootstrap */
.container-fluid {
  padding-right: 0;
  padding-left: 0;
  margin-right: auto;
  margin-left: auto;
}
/* Wrapper */
#wrapper {
  overflow: hidden;
}
.background-content {
  background-color: rgba(190, 195, 202, 0.3);
  height: 100%;
}
/* Custom Style */
.custom-card {
  background-color: transparent;
  border: none;
  font-size: 16pt;
}
.custom-card-text-name {
  margin-left: -10px;
  margin-top: -15px;
}
.custom-card-text-price {
  margin-left: -10px;
  margin-top: -20px;
}
.btn-custom {
  background-color: transparent;
  border: none;
}
/* Navbar */
.navbarOne {
  height: 70px;
  background-color: #ffffff;
  box-shadow: 0 4px 5px -2px gray;
  border-left: #cecece 1px solid;
  border-right: #cecece 1px solid;
  z-index: 1;
}
.navbarTwo {
  height: 70px;
  background-color: #ffffff;
  box-shadow: 0 4px 5px -2px gray;
  border-left: #cecece 1px solid;
  border-right: #cecece 1px solid;
  z-index: 1;
}
@media (max-width: 576px) {
  .navbarOne {
    box-shadow: none;
  }
  .navbarTwo {
    box-shadow: none;
  }
}
/* Sidemnu */
.sidemenu-box {
  width: 90px;
  height: 100%;
}
#sidemenu-wrapper {
  min-height: 100vh;
  margin-left: 0;
  -webkit-transition: margin 0.25s ease-out;
  -moz-transition: margin 0.25s ease-out;
  -o-transition: margin 0.25s ease-out;
  transition: margin 0.25s ease-out;
}
.sidemenu-header-box {
  height: 70px;
  font-size: 25px;
}
.modify-link-text {
  text-decoration: none;
  color: black;
}
.modify-link-text:hover {
  text-decoration: none;
  color: black;
}
#page-content-wrapper {
  width: 100%;
}
#wrapper.toggled #sidemenu-wrapper {
  /* margin-left: 0; */
  margin-left: -6rem;
}
/* Footer */
.footers {
  width: 100%;
  height: 50px;
}
</style>
