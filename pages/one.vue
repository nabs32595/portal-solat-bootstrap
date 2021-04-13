<template>
  <div>
    <div class="container">
      <div class="card card-1">
        <div id="demo1" class="carousel slide" data-ride="carousel">
          <!-- Indicators -->
          <ul class="carousel-indicators">
            <li data-target="#demo" data-slide-to="0" class="active"></li>
            <li data-target="#demo" data-slide-to="1"></li>
            <li data-target="#demo" data-slide-to="2"></li>
          </ul>
          <!-- The slideshow -->
          <div class="carousel-inner">
            <div class="carousel-item active">
              <div class="row">
                <div class="col-6">
                  <div class="temp">23&deg;</div>
                  <div class="location">Coimbra, Portugal</div>
                </div>
                <div class="col-6 justify-content-right">
                  <img
                    class="img-fluid"
                    src="https://img.icons8.com/plasticine/100/000000/sun.png"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="card card-2">
        <div id="demo2" class="carousel slide" data-ride="carousel">
          <!-- Indicators -->
          <ul class="carousel-indicators">
            <li data-target="#demo" data-slide-to="0"></li>
            <li data-target="#demo" data-slide-to="1" class="active"></li>
            <li data-target="#demo" data-slide-to="2"></li>
          </ul>
          <!-- The slideshow -->
          <div class="carousel-inner">
            <div class="carousel-item active">
              <div class="row">
                <div class="col">
                  <div class="row row1">21&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/ios/100/000000/sun.png"
                    />
                  </div>
                  <div class="row row3">12:00</div>
                  <div class="row row4">PM</div>
                </div>
                <div class="col">
                  <div class="row row1">20&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/ios/100/000000/sun.png"
                    />
                  </div>
                  <div class="row row3">1:00</div>
                  <div class="row row4">PM</div>
                </div>
                <div class="col">
                  <div class="row row1">20&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/windows/100/000000/cloud.png"
                    />
                  </div>
                  <div class="row row3">2:00</div>
                  <div class="row row4">PM</div>
                </div>
                <div class="col">
                  <div class="row row1">19&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/windows/100/000000/cloud.png"
                    />
                  </div>
                  <div class="row row3">3:00</div>
                  <div class="row row4">PM</div>
                </div>
                <div class="col">
                  <div class="row row1">18&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/cotton/64/000000/rain--v3.png"
                    />
                  </div>
                  <div class="row row3">4:00</div>
                  <div class="row row4">PM</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="card card-3">
        <div id="demo" class="carousel slide" data-ride="carousel">
          <!-- Indicators -->
          <ul class="carousel-indicators">
            <li data-target="#demo" data-slide-to="0"></li>
            <li data-target="#demo" data-slide-to="1"></li>
            <li data-target="#demo" data-slide-to="2" class="active"></li>
          </ul>
          <!-- The slideshow -->
          <div class="carousel-inner">
            <div class="carousel-item active">
              <div class="row">
                <div class="col">
                  <div class="row row1">21&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/ios/100/000000/sun.png"
                    />
                  </div>
                  <div class="row row3">Mon</div>
                </div>
                <div class="col">
                  <div class="row row1">20&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/ios/100/000000/sun.png"
                    />
                  </div>
                  <div class="row row3">Tue</div>
                </div>
                <div class="col">
                  <div class="row row1">16&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/windows/100/000000/cloud.png"
                    />
                  </div>
                  <div class="row row3">Wed</div>
                </div>
                <div class="col">
                  <div class="row row1">17&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/windows/100/000000/cloud.png"
                    />
                  </div>
                  <div class="row row3">Thu</div>
                </div>
                <div class="col">
                  <div class="row row1">18&deg;</div>
                  <div class="row row2">
                    <img
                      class="img-fluid"
                      src="https://img.icons8.com/cotton/64/000000/rain--v3.png"
                    />
                  </div>
                  <div class="row row3">Fri</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
body {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(238, 237, 237, 0.438);
  color: rgb(105, 104, 104);
  font-family: sans-serif;
}

.container {
  width: fit-content;
}

.card {
  padding: 1.2rem 3rem 1rem 3rem;
  margin: 1rem;
  border-radius: 1.5rem;
  border-color: rgba(238, 237, 237, 0.438);
  box-shadow: 5px 8px 10px #80808033;
}

@media (max-width: 767px) {
  .card {
    height: 10rem;
    padding: 1.5rem 1.5rem 1rem 1.5rem;
  }
}

.carousel-indicators li {
  width: 5px;
  height: 6px;
  border-radius: 100%;
  opacity: 0.2;
  background-color: #000000;
}

.carousel-indicators {
  margin-bottom: 0;
}

.temp {
  font-size: 5rem;
  color: rgb(57, 57, 58);
}

.card-1 {
  background: linear-gradient(
    to right,
    #ffffff 50%,
    rgba(241, 224, 190, 0.507)
  );
}

@media (max-width: 767px) {
  .temp {
    font-size: 3rem;
  }
}

.location {
  margin-bottom: 1.5rem;
}

@media (max-width: 767px) {
  .location {
    font-size: 0.75rem;
  }
}

.img-fluid {
  float: right;
  width: 65%;
  display: flex;
  align-items: center;
}

.row2 .img-fluid {
  margin: 10% 0;
  opacity: 0.5;
  width: 40%;
}

.card-2 .row {
  justify-content: center;
}

.card-3 .row {
  justify-content: center;
}

.row1 {
  font-size: 0.7rem;
  font-weight: bold;
  color: black;
}

.row3 {
  font-size: 0.9rem;
  font-weight: bold;
  color: black;
}

@media (max-width: 400px) {
  .row3 {
    font-size: 0.7rem;
    font-weight: bold;
    color: black;
  }
}

@media (max-width: 320px) {
  .row3 {
    font-size: 0.6rem;
    font-weight: bold;
    color: black;
  }
}

.row4 {
  font-size: 0.6rem;
  color: rgb(196, 196, 196);
  margin: 5% 0 2.5rem;
}

.card-3 .row3 {
  margin: 5% 0 2.5rem;
}

.col {
  overflow: visible;
}

.row {
  overflow: visible;
}
</style>
