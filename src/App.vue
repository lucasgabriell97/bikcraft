<template>
  <div id="app">
    <TheHeader/>
    <router-view></router-view>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'

export default {
  name: 'App',
  components: {
    TheHeader
  }
}
</script>

<style>
/*==== RESET ====*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  padding-bottom: 600px;
  color: #111;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  color: inherit;
}

img {
  max-width: 100%;
  display: block;
} 

/*==== MAIN BUTTON ====*/
.button {
  display: inline-block;
  padding: 16px 32px;
  background: linear-gradient(#ffbf00, #f2a50c);
  border-radius: 4px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0,1);
  text-transform: uppercase;
  color: #332200;
  font: 600 1.125rem/1.35 "Poppins", sans-serif;
}

.button:hover {
  background: linear-gradient(#ffb60d, #e59317);
}

@media (max-width: 600px) {
  .button {
    padding: 12px 16px;
    font-size: 1rem;
  }
}

/*==== UTILITIES ====*/
.font-1-xs {
  font: 400 0.75rem/1.35 "Poppins", sans-serif;
}

.font-2-xs {
  font: 400 0.875rem/1.43 "Roboto", sans-serif;
}

.font-1-s {
  font: 400 1rem/1.5 "Poppins", sans-serif;
}

.font-2-s {
  font: 400 1rem/1.5 "Roboto", sans-serif;
}

.font-1-m,
.font-1-m-b {
  font: 400 1.125rem/1.35 "Poppins", sans-serif;
}

.font-1-m-b {
  font-weight: 600;
}

.font-2-m {
  font: 500 1.125rem/1.35 "Roboto", sans-serif;
}

.font-1-l {
  font: 400 1.5rem/1.5 "Poppins", sans-serif;
}

.font-2-l,
.font-2-l-b {
  font: 400 1.5rem/1.5 "Roboto", sans-serif;
}

.font-2-l-b {
  font-weight: 500;
  letter-spacing: 0.015em;
  text-transform: uppercase;
}

.font-1-xl {
  font: 600 2rem/1.25 "Poppins", sans-serif;
}

.font-2-xl {
  font: 500 2rem/1.25 "Roboto", sans-serif;
  
}

.font-1-xxl {
  font: 600 4rem/1.125 "Poppins", sans-serif;
}

@media (max-width: 1200px) {
  .font-1-xxl {
    font-size: 3rem;
  }
  
  .font-2-l,
  .font-2-l-b {
    font-size: 1.125rem;
  }
}

@media (max-width: 800px) {
  .font-1-xxl {
    font-size: 2rem;
  }

  .font-1-xl,
  .font-2-xl {
    font-size: 1.5rem;
  }
}

:root {
  --primary-color: #ffbb00;
  --black-color: #000;
  --white-color: #fff;
  --gray-color-text: #b2b2b2;
  --gray-color-bg: #111;
}

.primary-color {
  color: #ffbb00;
}
</style>