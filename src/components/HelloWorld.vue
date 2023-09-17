<template>
  <v-container class="mt-14" id="home">
    <div>
      <div class="d-flex justify-center align-center">
        <div>
          <div>
            <h1 class="f-title">Front-End Software Developer</h1>
          </div>
          <br />
          <div>
            Resolving development problems, building smart user interfaces and
            useful interactions, developing rich web applications and seamless
            web experiences.
          </div>
        </div>
        <div class="bg d-flex justify-center align-center">
          <div class="multicolortext">
            var hero = { _name: 'John Doe',
            <br />
            getSecretIdentity: function (){ return this._name; } };
            <br />
            var stoleSecretIdentity = hero.getSecretIdentity;
          </div>
        </div>
      </div>
    </div>

    <div class="mt-8">
      <v-btn variant="outlined">
        <a href="#front-dev">Know me more</a>
        <v-icon>mdi-chevron-down</v-icon>
      </v-btn>
    </div>
  </v-container>
</template>

<script setup>
//
</script>

<style scoped>
@media only screen and (max-width: 570px) {
  .bg {
    width: 40% !important;
    height: 190px !important;
  }

  .multicolortext {
    font-size: 6px !important;
  }
}
.bg {
  transform: rotate3d(1, 4, 1, 50deg);
  box-shadow: 0 3px 10px rgba(29, 32, 206, 0.541);
  width: 50%;
  height: 250px;
  border: 1px solid white;
  border-image: linear-gradient(
      rgb(179, 44, 186),
      rgb(255, 247, 247),
      blue,
      rgb(255, 247, 247)
    )
    27 / 5px;
  animation: animateColor 2s ease-in-out infinite;
}

@keyframes animateColor {
  50% {
    border-image: linear-gradient(
        rgb(179, 44, 186),
        blue,
        rgb(255, 247, 247),
        rgb(134, 36, 139)
      )
      27 / 5px;
  }
  75% {
    border-image: linear-gradient(
        blue,
        rgb(255, 247, 247),
        blue,
        rgb(255, 247, 247)
      )
      27 / 5px;
  }
}

.multicolortext {
  background-image: linear-gradient(
    to left,
    violet,
    rgb(255, 255, 255),
    green,
    rgb(255, 255, 255),
    yellow,
    orange,
    red
  );
  padding: 26px;
  overflow: hidden;
  letter-spacing: 2px;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  background-clip: text;
  color: transparent;
}

.f-title {
  background-image: linear-gradient(to left, rgb(0, 0, 0), rgb(255, 255, 255));
  animation: animateText 3s ease-in-out infinite;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  background-clip: text;
  color: transparent;
}

@keyframes animateText {
  75% {
    background-image: linear-gradient(
      to right,
      rgb(0, 0, 0),
      rgb(255, 255, 255)
    );
  }
}
</style>