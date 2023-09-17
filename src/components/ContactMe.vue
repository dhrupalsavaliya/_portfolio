<template>
  <v-container class="mt-14 mb-8">
    <div id="cont">
      <div class="d-flex justify-center align-center flex-column contact">
        <h1>GET IN TOUCH</h1>

        <div>
          <v-icon>mdi-email-arrow-right</v-icon>

          dhrupalsavaliya09@gmail.com
        </div>

        <div>
          <v-icon>mdi-cellphone-message</v-icon>
          9106373172
        </div>

        <div>
          <div class="d-flex justify-center align-center icons">
            <div>
              <a
                href="https://www.linkedin.com/in/dhrupal-savaliya-110a051a2"
                target="_blank"
                ><img
                  width="40"
                  height="40"
                  src="https://img.icons8.com/color/40/000000/linkedin.png"
                  alt="linkedin"
              /></a>
            </div>
            <div>
              <a href="https://github.com/Dhrupal-albiorix" target="_blank">
                <img
                  width="40"
                  height="40"
                  src="https://img.icons8.com/plasticine/40/github.png"
                  alt="github"
                />
              </a>
            </div>
            <div>
              <a href="https://medium.com/@dhrupalsavaliya09" target="_blank">
                <img
                  width="40"
                  height="40"
                  src="https://img.icons8.com/arcade/40/medium-logo.png"
                  alt="medium-logo"
                />
              </a>
            </div>
            <div>
              <a href="#" target="_blank">
                <img
                  width="40"
                  height="40"
                  src="https://img.icons8.com/bubbles/40/reddit.png"
                  alt="reddit"
                />
              </a>
            </div>
          </div>
        </div>

        <img src="../assets/tea-cup.gif" alt="" class="footer-img" />
      </div>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style scoped>
.contact,
.icons {
  gap: 20px;
}

.footer-img {
  width: 18%;
}
</style>