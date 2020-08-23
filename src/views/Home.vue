<template>
  <div id="wrapper">
    <b-container fluid>
      <!-- Header -->
      <nav>
        <b-row>
          <b-col xl="8" md="7" sm="7" class="navbarOne">One</b-col>
          <b-col xl="4" md="5" sm="5" class="navbarTwo">Two</b-col>
        </b-row>
      </nav>
      <!-- End Header -->
      <!-- Content -->
      <b-row>
        <b-col xl="12" class="background-content">
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
                      img-src="https://picsum.photos/300/220/?image=41"
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
                      img-src="https://picsum.photos/300/220/?image=41"
                      img-alt="Image"
                      img-top
                      class="custom-card"
                    >
                      <b-card-text class="custom-card-text-name font-book">Coffee Latte</b-card-text>
                      <b-card-text class="custom-card-text-price font-medium">Rp. 15.000</b-card-text>
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
            <b-col xl="8" md="7" sm="7" style="background-color: blue;"></b-col>
            <!-- End Cart -->
          </b-row>
        </b-col>
      </b-row>
      <!-- End Content -->
    </b-container>
  </div>
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
}
@media (max-width: 576px) {
  .navbarOne {
    box-shadow: none;
  }
  .navbarTwo {
    box-shadow: none;
  }
}
/* End Navbar */
</style>
