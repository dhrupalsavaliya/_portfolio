<template>
  <v-container class="mt-14 intropage" id="front-dev">
    <div>
      <v-spacer class="devide"> </v-spacer>

      <div class="intro">
        <div class="content">
          <div>
            <h1>
              Hi, I'm Dhrupal ,
              <br />
              WebDeveloper
            </h1>
          </div>
          <div>Front End Developer / JavaScript Fan</div>
        </div>
        <div class="cube">
          <div class="top">{...}</div>
          <div class="right">JSON</div>
          <div class="bottom">[]</div>
          <div class="left">Stringfy</div>
          <div class="front">&&</div>
          <div class="back">||</div>
        </div>

        <div class="content">
          <div>Professionally connected with the web development industry.</div>

          <div>
            Problem solver, well-organised person, loyal employee with high
            attention to detail.
          </div>

          <div>
            Fan of sci-fi thrills, spiritual exploration, storytelling, Book
            reading , music , and coding of course
          </div>

          <div>
            Interested in the entire frontend spectrum and working on ambitious
            projects with interesting people.
          </div>
        </div>
      </div>
      <v-spacer class="devide"></v-spacer>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style scoped>
@media only screen and (max-width: 600px) {
  .intro {
    flex-wrap: wrap !important;
  }
  .cube {
    margin-left: 70% !important;
    margin-top: 2% !important;
  }
}

.intro {
  gap: 50px;
  width: 100%;
  display: flex;
  flex-wrap: nowrap;
}

.intro .content {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  gap: 12px;
  flex-wrap: wrap;
}

.devide {
  margin-top: 120px;
}

.cube {
  -webkit-transform-style: preserve-3d;
  -webkit-animation: spin 20s infinite ease-out;
  position: relative;
  width: 100px;
  height: 100px;
  top: -10%;
  right: 10%;
  margin-left: -50px;
  margin-top: -50px;
}

.cube div {
  width: 100px;
  height: 100px;
  line-height: 100px;
  text-align: center;
  box-shadow: inset 0px 0px 0px 1px rgba(10, 0, 0, 0.8);
  border: 2px solid white;
  display: block;
  position: absolute;
}

.cube div.top {
  -webkit-transform: rotateX(90deg);
  margin-top: -50px;
}

.cube div.right {
  -webkit-transform: rotateY(90deg);
  margin-left: 50px;
}

.cube div.bottom {
  -webkit-transform: rotateX(-90deg);
  margin-top: 50px;
}

.cube div.left {
  -webkit-transform: rotateY(-90deg);
  margin-left: -50px;
}

.cube div.front {
  -webkit-transform: translateZ(50px);
}

.cube div.back {
  -webkit-transform: translateZ(-50px) rotateX(180deg);
}

@-webkit-keyframes spin {
  0% {
    -webkit-transform: rotateX(-20deg) rotateY(20deg);
  }
  100% {
    -webkit-transform: rotateX(-20deg) rotateY(780deg);
  }
}
</style>