<template>
  <div class="thanks">
    <h1>Thank you</h1>
    <div class="thank-you-message">
      <div>Thank you for reading my work til the end. I’d love to hear what you think!</div>
      <br>
      <div>
        Shoot me a message on <a href="https://www.linkedin.com/in/jesse-ting-b2a383128/">LinkedIn</a> or send me an <a href="mailto:jessedingx2@gmail.com">email</a> to tell me your thought.
      </div>
    </div>
  </div>
</template>

<style scoped>
.thanks {
  margin-top: 13em;
  margin-bottom: 13em;
}

.thanks h1 {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 500;
  font-size: 70px;
  text-align: center;
  color: #1A3163;
}

.thank-you-message {
  margin-top: 1em;
}

.thank-you-message div {
  font-family: Karla;
  font-style: normal;
  font-weight: 300;
  font-size: 30px;
  line-height: 35px;

  text-align: center;
}

@media (max-width: 420px) {
  .thanks {
    margin-bottom: 4em;
  }

  .thanks h1 {
    font-size: 40px;
  }

  .thank-you-message div {
    font-size: 20px;
  }
}

</style>
