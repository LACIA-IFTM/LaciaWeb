---------------------------------------TEMPLATE---------------------------------------
<template>
  <header id="topBar" class="topBarClass">
    <nav>
      <ul class="nav-list">
        <li class="nav-item"><a href="#">HOME</a></li>
        <li class="nav-item"><a href="#">CURSOS</a></li>
        <li class="nav-item"><a href="#">PROJETOS</a></li>
        <li class="nav-item"><a href="#">JOBS</a></li>
        <li class="nav-item"><a href="#">SOBRE</a></li>
      </ul>
    </nav>
  </header>
  <div class="main-content">
    <section class="section black-section">
      <h2>Seção 1</h2>
      <p>Conteúdo da primeira seção.</p>
    </section>
    <section class="section blue-section">
      <h2>Seção 2</h2>
      <p>Conteúdo da segunda seção.</p>
    </section>
    <section class="section white-section">
      <h2>Seção 3</h2>
      <p>Conteúdo da terceira seção.</p>
    </section>
  </div>
  <footer class="footer">
    <p>© 2024 Meu Site. Todos os direitos reservados.</p>
  </footer>
</template>

---------------------------------------SCRIPTS----------------------------------------
<script>
export default {
  name: 'HomePage'
}
</script>


----------------------------------------STYLES----------------------------------------
<style scoped>
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  overflow-x: hidden; /* Evita o scroll horizontal */
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.topBarClass {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  background-color: #000912;
  padding: 0 20px;
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1000;
}

.nav-list {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

.nav-item {
  margin-right: 20px;
}

.nav-item a {
  color: #ffffff;
  text-decoration: none;
  font-size: 18px;
}

.nav-item a:hover {
  text-decoration: underline;
}

.main-content {
  flex: 1;
  width: 100%;
  box-sizing: border-box; /* Inclui padding e border no cálculo da largura */
  padding-top: 100px; /* Para evitar que o conteúdo fique escondido atrás da barra fixa */
}

.section {
  padding: 50px;
  text-align: center;
  width: 100%;
  box-sizing: border-box; /* Inclui padding e border no cálculo da largura */
}

.black-section {
  background-color: #000000;
  color: #ffffff;
}

.blue-section {
  background-color: #0000ff;
  color: #ffffff;
}

.white-section {
  background-color: #ffffff;
  color: #000000;
}

.footer {
  background-color: #000912;
  color: #ffffff;
  text-align: center;
  padding: 20px;
  width: 100%;
  position: relative;
  bottom: 0;
}

/* Media Queries para Responsividade */
@media (max-width: 768px) {
  .topBarClass {
    flex-direction: column;
    height: auto;
    padding: 10px;
  }

  .nav-list {
    flex-direction: column;
    align-items: center;
  }

  .nav-item {
    margin: 10px 0;
  }

  .section {
    padding: 20px;
  }
}
</style>

