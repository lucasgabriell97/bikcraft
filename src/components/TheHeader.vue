<template>
  <header class="header-bg">
    <div class="header">
      <router-link to="/">
        <img src="../assets/img/bikcraft.svg" alt="Bikcraft">
      </router-link>
      <nav aria-label="primary">
        <ul class="header-menu font-1-m">
          <li><router-link to="/bicicletas.html">Bicicletas</router-link></li>
          <li><router-link to="/seguros.html">Seguros</router-link></li>
          <li><router-link to="/contato.html">Contato</router-link></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'TheHeader'
}
</script>

<style scoped>
.header-bg {
  background-color: var(--black-color);
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;

  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
}

.header-menu {
  display: flex;
  flex-wrap: wrap;
  gap: 40px;
}

.header-menu a {
  display: inline-block;
  padding: 16px 0;
  color: var(--white-color);
  position: relative;
}

.header-menu a:after {
  content: "";
  position: absolute;
  display: block;
  height: 2px;
  width: 0px;
  background-color: var(--white-color);
  margin-top: 4px;
  transition: width 0.3s ease-out;
}

.header-menu a:hover:after {
  width: 100%;
}

@media (max-width: 800px) {
  .header-menu {
    gap: 20px;
  }

  .header-menu a {
    background-color: var(--gray-color-bg);
    padding: 12px 16px;
    border-radius: 4px;
  }

  .header-menu a:hover {
    background-color: #2e2e2e;
  }

  .header a:after {
    display: none;
  }
}

@media (max-width: 600px) {
  .header-menu {
    gap: 12px;
  }

  .header-menu a {
    padding: 8px 12px;
    font-size: 0.875rem;
  }
}
</style>
