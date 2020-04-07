<template>
  <div class="footer">
    <div class="footer-center">
      <div class="letstalk">
        Get in touch with me
      </div>
      <div>
        <a href="https://www.linkedin.com/in/jesse-ting-b2a383128/">
          <img src="~assets/linkedin.png"></a>
        <a href="mailto:jessedingx2@gmail.com"><img src="~assets/email.png"></a>
        <a href="https://www.facebook.com/jd.harrison.568">
          <img src="~assets/facebook.png"></a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.footer {
  text-align: center;
  background-color: #1A3163;
  height: 258px;
  position: relative;
}

.footer-center {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.letstalk {
  color: white;
  font-family: Karla;
  font-style: normal;
  font-weight: bold;
  font-size: 25px;
  line-height: 29px;
  align-items: center;
}

.footer img {
  padding: 1em;
}
</style>
