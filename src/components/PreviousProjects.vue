<template>
  <v-container class="mt-14">
    <v-carousel
      :continuous="true"
      :show-arrows="true"
      hide-delimiter-background
      hide-delimiters
      height="300"
      class="mt-12"
    >
      <v-carousel-item>
        <div>
          <div class="mt-2 d-flex justify-center align-center project">
            <div class="sphere">
              <div class="text-center mt-10">
                <h1>Projects <v-icon>mdi-arrow-right-bold-circle</v-icon></h1>
              </div>
            </div>
          </div>
        </div>
      </v-carousel-item>

      <v-carousel-item>
        <div class="d-flex justify-center align-center flex-column project">
          <div>
            <div class="about-project">
              I have built various different projects to fit different aspects.
              I have used Vue ,node ,Express , mongoDB , mongoose , GraphQl to
              build those Projects.
            </div>
          </div>
          <div class="text-center">
            See Projects
            <v-icon>mdi-arrow-right-bold-circle</v-icon>
          </div>
        </div>
      </v-carousel-item>

      <v-carousel-item> </v-carousel-item>

      <v-carousel-item> 14 </v-carousel-item>
    </v-carousel>
  </v-container>
</template>

<script>
export default {};
</script>

<style scoped>
.project {
  gap: 20px;
}

.sphere {
  animation: spin 6.66s linear infinite;
  border: 1px dotted rgb(222, 222, 22);
  border-radius: 50%;
  height: 150px;
  position: relative;
  transform-style: preserve-3d;
  width: 150px;
}
.sphere:hover {
  border: 1px dotted rgb(22, 222, 222);
  transition: 0.666s border;
}
.sphere::before,
.sphere::after {
  border: 1px dotted rgb(222, 222, 22);
  border-radius: 50%;
  content: "";
  height: 150px;
  left: 0;
  position: absolute;
  top: 0;
  width: 150px;
}
.sphere:hover::before,
.sphere:hover::after {
  border: 1px dotted rgb(22, 222, 222);
  transition: 0.666s border;
}
.sphere::before {
  transform: rotateX(-66.6deg);
}
.sphere::after {
  transform: rotateX(66.6deg);
}

@keyframes spin {
  0% {
    transform: rotateY(0deg) rotateX(0deg) rotateZ(0deg);
  }
  100% {
    transform: rotateY(360deg) rotateX(360deg) rotateZ(360deg);
  }
}

.about-project {
  width: 40%;
  margin-left: 31%;
  text-align: center;
}

@media only screen and (max-width: 780px) {
  .about-project {
    width: 100%;
    margin-left: 0%;
  }
}
</style>