<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

@media (min-width: 421px) {
 .padded {
    margin-left: 10%;
    margin-right: 10%;
 }
}

.break {
  padding-bottom: 7.5em;
}

@media (max-width: 420px) {
  .break {
      padding-bottom: 2em;
  }
}

.main-description {
  margin-top: 5em;
}

@media(max-width: 420px) {
  .main-description {
    margin-top: 1em;
  }
}

.grey-header-small {
  font-family: Karla;
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 58px;

  display: flex;
  align-items: center;

  color: #666666;

  border-top: 1px solid #DDDDDD;

  margin-top: 1em;
}

@media (max-width: 420px) {
  .grey-header-small {
    font-size: 12px;
    line-height: 32px;
  }
}

</style>
