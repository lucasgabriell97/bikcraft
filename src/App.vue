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
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
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

.introduction-bg {
  background-color: #000;
  color: #fff;
}

.introduction {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0 40px;
  max-width: 1200px;
  padding: 0 20px;
  margin: 0 auto;
}

.introduction-content {
  align-self: end;
  padding-bottom: 80px;
}

.introduction h1 {
  margin-bottom: 32px;
  font-size: 4rem;
  line-height: 72px;
}

.introduction h1 span {
  color: #ffbb00;
}

.introduction p {
  margin-bottom: 20px;
  font-size: 1.5rem;
  line-height: 36px;
  color: #b2b2b2;
}

.introduction a {
  display: inline-block;
  padding: 16px 32px;
  background: linear-gradient(#ffbf00, #f2a50c);
  border-radius: 4px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0,1);
  text-transform: uppercase;
  color: #332200;
  font-size: 1.125rem;
  font-weight: bold;
  line-height: 1.33;
}

.introduction a:hover {
  background: linear-gradient(#ffb60d, #e59317);
}

</style>