<script setup></script>

<style lang="scss">
@font-face {
  font-family: 'Sofia Pro';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url('./assets/fonts/SOFIA-PRO-REGULAR-AZ.OTF') format('truetype');
}

@font-face {
  font-family: 'Sofia Pro';
  font-style: medium;
  font-weight: 500;
  font-display: swap;
  src: url('./assets/fonts/SOFIA-PRO-MEDIUM-AZ.OTF') format('truetype');
}

@font-face {
  font-family: 'Sofia Pro';
  font-style: bold;
  font-weight: 700;
  font-display: swap;
  src: url('./assets/fonts/SOFIA-PRO-BOLD-AZ.OTF') format('truetype');
}

$bg: #161621;
$card-bg: #1e1f36;
$white: #f8f8f8;
$cta: #4346d4;
$text: #8e8faf;
$dark: #232443;
$dark-rectangle: hsla(238, 31%, 20%, 0.5);

#app {
  font-family: Sofia Pro, Roboto, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
}

body,
body::before,
body::after {
  margin: 0;
  padding: 0;
  background: $bg;
}

p,
a {
  color: $text;
}

h1 {
  color: $white;
  font-size: 1.5em;
}

img {
  height: 1.8rem;
}

a {
  text-decoration: none;
  font-size: 1.3em;
  transition: all ease 0.3s;

  &:hover {
    color: #11affe;
  }
}

header {
  display: flex;
  align-content: center;
  align-items: center;
  justify-content: space-between;
  padding: 0rem 1rem;
  a {
    margin-left: 2rem;
  }
}

.wrapper {
  padding: 2rem 1rem;
}

.card-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
  width: 100%;
  margin: auto;
}

.card {
  text-align: center;
  background: $card-bg;
  padding: 4rem 1.5rem;
  border-radius: 8px;
  width: 80%;

  #description {
    margin-top: 2rem;
    font-size: 1em;
  }
}

.cta-wrapper {
  background: none;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;
  padding: 0rem 1rem;
  font-family: inherit;
  margin-top: 2rem;
  p {
    display: none;
  }

  button {
    cursor: pointer;
    border: none;
    background: $cta;
    color: $white;
    padding: 0.5rem 1rem;
    font-style: medium;
    font-weight: 500;
    font-size: 0.7em;
    font-family: inherit;
    border-radius: 2px;
  }
}
</style>

<template>
  <div class="wrapper">
    <header>
      <img src="./assets/logo_white_text.png" alt="MingoDesk logo with the MingoDesk name in text" />
      <a href="https://github.com/MingoDesk/">Github</a>
    </header>
    <main>
      <div class="card-container">
        <div class="card">
          <img src="./assets/logo.png" alt="MingoDesk logo" />
          <h1>The simple yet powerful helpdesk.</h1>
          <p id="description">
            MingoDesk has everything you need to support your customers in an easy and consistent way. The application
            also provides powerful analytical tools to help you work proactively.
          </p>
          <div class="cta-wrapper">
            <p>Get notified when the beta is here</p>
            <div class="button-container">
              <a href="https://forms.gle/vno3LyuPr9MdjWuFA" target="_blank"><button>Join the waitlist</button></a>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>
