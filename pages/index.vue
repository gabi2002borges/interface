<template>
  <container>
      <div class="line"></div>
      <header class="menu">
        <section class="imagem_logo">
          <img src="/logo.png" alt="logo_ets" />
        </section>
        <section class="meio_header"></section>
        <section class="list">
          <div class="links">
            <a class="link" href="#">Catalogo</a>
            <a class="link" href="#">Search</a>
            <a class="link" href="#">Admin</a>
          </div>
        </section>
      </header>

    <footer class="rodape">
      <h4>© Robert Bosch Ltda. 2022, all rights reserved</h4>
    </footer>
  </container>
</template>

<script>
export default {
  name: 'mm21',
}
</script>

<style lang="scss" scoped>


body {
  height: 100%;
  width: 100%;
}

 .menu {
  height: 70px;
  width: 100%;
  display: flex;
  flex-direction: row;
}


.meio_header {
  height: 100%;
  width: 60%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  background-color: white;
}

.list {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  background-color: white;
  font-weight: 600;
  padding-inline-start: 0px;
}

.link {
  position: relative;
  padding-bottom: 8px;
  cursor: pointer;
  color: black;
  padding: 0 2px;
  margin: 0 15px;
  text-decoration: none;
}

.line {
  margin-top: 0;
  height: 1rem;
  background-image: url('/linha.jfif');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
}

.imagem_logo {
  height: 100%;
  width: 15%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: white;
}

</style>