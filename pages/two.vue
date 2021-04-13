<template>
  <div class="container d-flex justify-content-center">
    <div class="weather">
      <div class="row">
        <div class="col-md-6">
          <div class="card">
            <span class="icon"
              ><img
                class="img-fluid"
                src="https://img.icons8.com/emoji/96/000000/sun-emoji.png"
            /></span>
            <div class="title">
              <p>Sydney</p>
            </div>
            <div class="temp">+20<sup>&deg;</sup></div>
            <div class="row">
              <div class="col-4">
                <div class="header">General</div>
                <div class="value">Sunny</div>
              </div>
              <div class="col-4">
                <div class="header">Air pollution</div>
                <div class="value">47</div>
              </div>
              <div class="col-4">
                <div class="header">Fire</div>
                <div class="value">No</div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="card">
            <span class="icon"
              ><img
                class="img-fluid"
                src="https://img.icons8.com/emoji/96/000000/sun-emoji.png"
            /></span>
            <div class="title">
              <p>Melbourne</p>
            </div>
            <div class="temp">+18<sup>&deg;</sup></div>
            <div class="row">
              <div class="col-4">
                <div class="header">General</div>
                <div class="value">Sunny</div>
              </div>
              <div class="col-4">
                <div class="header">Air pollution</div>
                <div class="value">20</div>
              </div>
              <div class="col-4">
                <div class="header">Fire</div>
                <div class="value">No</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <div class="card">
            <span class="icon"
              ><img src="https://img.icons8.com/color/50/000000/wind.png"
            /></span>
            <div class="title">
              <p>Lithgow</p>
            </div>
            <div class="temp">+17<sup>&deg;</sup></div>
            <div class="row">
              <div class="col-4">
                <div class="header">General</div>
                <div class="value">Wind</div>
              </div>
              <div class="col-4">
                <div class="header">Air pollution</div>
                <div class="value">52</div>
              </div>
              <div class="col-4">
                <div class="header">Fire</div>
                <div class="value">No</div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="card">
            <span class="icon"
              ><img
                src="https://img.icons8.com/office/80/000000/partly-cloudy-day.png"
            /></span>
            <div class="title">
              <p>Darvin</p>
            </div>
            <div class="temp">+15<sup>&deg;</sup></div>
            <div class="row">
              <div class="col-4">
                <div class="header">General</div>
                <div class="value">Cloudy</div>
              </div>
              <div class="col-4">
                <div class="header">Air pollution</div>
                <div class="value">34</div>
              </div>
              <div class="col-4">
                <div class="header">Fire</div>
                <div class="value">No</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Two',
}
</script>

<style scoped>
body {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(238, 237, 237, 0.33);
  color: rgb(105, 104, 104);
  font-family: sans-serif;
}

.container {
  height: 80vh;
  background-color: #ffffff;
  border-color: #ffffff;
  align-items: center;
  border-radius: 1rem;
  vertical-align: middle;
}

@media (max-width: 767px) {
  .container {
    height: fit-content;
  }
}

.weather {
  width: 77%;
}

@media (max-width: 767px) {
  .weather {
    width: 100%;
  }
}

.card {
  padding: 1rem;
  margin: 1.5rem 4vw;
  border-radius: 1rem;
  background-color: rgba(238, 237, 237, 0.22);
  border-color: rgba(238, 237, 237, 0.22);
  box-shadow: 5px 6px 6px 2px #e9ecef;
  text-align: center;
}

@media (max-width: 768px) {
  .card {
    margin: 1.5rem;
  }
}

.title {
  justify-content: center;
  position: absolute;
  left: 50%;
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);
}

.title p {
  margin-bottom: 0.2rem;
  font-size: 1.2rem;
}

.temp {
  font-size: 2.6rem;
  margin-bottom: 1rem;
}

.header {
  color: #dddddd;
}

.col-4 {
  padding: 0 0.2rem;
}

.icon {
  align-self: flex-end;
  margin-right: -2.5rem;
  margin-top: -2rem;
  z-index: 999;
}

.icon img {
  width: 5rem;
}
</style>
