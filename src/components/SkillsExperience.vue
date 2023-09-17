<template>
  <v-container>
    <div>
      <div class="skill-intro">
        <div class="text-center title mt-2">
          "A PROBLEM IS A CHANCE FOR YOU TO DO YOUR BEST"
        </div>
        <h1 class="text-center title mt-2">Skills & Experience</h1>
        <div class="text-center">
          The main area of expertise is front end development (client side of
          the web)
        </div>
        <div>
          <div class="text-center skill-set">
            HTML, CSS, JS, building small and medium web applications with Vue
            or React, custom plugins, features, animations, and coding
            interactive layouts. I have also full-stack developer experience
            with Node , express , MongoDB and vue
          </div>
        </div>
      </div>

      <div>
        <v-row class="mt-8">
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/css3.png"
              alt="css3"
            />
          </v-col>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/sass.png"
              alt="sass"
            />
          </v-col>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/bootstrap.png"
              alt="bootstrap"
            />
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/javascript--v1.png"
              alt="javascript--v1"
            />
          </v-col>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/vue-js.png"
              alt="vue-js"
            />
          </v-col>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/office/96/react.png"
              alt="react"
            />
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/nodejs.png"
              alt="nodejs"
            />
          </v-col>

          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/fluency/96/graphql.png"
              alt="graphql"
          /></v-col>
          <v-col cols="12" md="4" class="text-center">
            <img
              width="96"
              height="96"
              src="https://img.icons8.com/color/96/mongodb.png"
              alt="mongodb"
            />
          </v-col>
        </v-row>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style scoped>
.title {
  letter-spacing: 2px;
}

.skill-intro {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  width: 100%;
  gap: 20px;
}

.skill-set {
  width: 60%;
  margin-left: 20%;
}
</style>