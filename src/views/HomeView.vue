<template>
  <main class="introduction-bg">
    <div class="introduction">
      <div class="introduction-content">
        <h1 class="font-1-xxl">Bicicletas feitas sob medida<span class="primary-color">.</span></h1>
        <p class="font-2-l">Bicicletas elétricas de alta precisão e qualidade, feitas sob medida para você. Explore o mundo na sua velocidade com a Bikcraft.</p>
        <router-link class="button" to="/bicicletas.html">Escolha a sua</router-link>
      </div>
      <div>
        <img src="../assets/img/fotos/introducao.jpg" alt="Bicicleta elétrica preta.">
      </div>
    </div>
  </main>

  <h2 class="font-1-xxl">escolha a sua<span class="primary-color">.</span></h2>
</template>

<script>
export default {
  name: "HomeView"
}
</script>

<style scoped>
.introduction-bg {
  background-color: var(--black-color);
  color: var(--white-color);
  box-shadow: inset 0 -120px var(--white-color);
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
  padding-bottom: 200px;
}

.introduction img {
  height: 100%;
  object-fit: cover;
  border-radius: 4px;
}

.introduction h1 {
  margin-bottom: 32px;
}

.introduction p {
  margin-bottom: 20px;
  color: var(--gray-color-text);
}

@media (max-width: 800px) {
  .introduction-bg {
    background-color: var(--gray-color-bg);
    padding-top: 40px;
    box-shadow: inset 0 -60px var(--white-color);
  }

  .introduction {
    grid-template-columns: 1fr;
    gap: 32px;
  }

  .introduction-content {
    padding-bottom: 0;
  }

  .introduction h1 {
    margin-bottom: 16px;
  }

  .introduction img {
    height: 300px;
    width: 100%;
  }
}
</style>