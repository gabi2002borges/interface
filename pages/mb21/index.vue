<template>
  <container>
    <header class="menu">
      <section class="imagem_logo">
        <img src="/logo.png" alt="logo_ets" />
      </section>
      <section class="meio"></section>
      <section class="list">
        <div class="links">
          <a class="link" href="#">Cavitoriatalog</a>
          <a class="link" href="#">Search</a>
          <a class="link" href="#">Consult</a>
          <a class="link" href="#">Contact</a>
        </div>
      </section>
    </header>

    <div class="line"></div>

    <main>
    </main>

    <footer>
      <h4>© Robert Bosch Ltda. 2022, all rights reserved</h4>
    </footer>
  </container>
</template>

<script>
export default {
  name: 'mm21',
}
</script>

<style lang="css" scoped>
.menu {
  height: 70px;
  width: 100%;
  display: flex;
  flex-direction: row;
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

.meio {
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
.links {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
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

.link::after {
  position: absolute;
  margin-bottom: -10px;
  bottom: 0;
  left: 0;
  content: '';
  width: 0%;
  height: 3px;
  background-color: red;
  transition: width 0.4s ease-out;
}

.link:hover.link::after {
  width: 100%;
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

main {
  background-color: rgb(102, 7, 55);
  height:85vh;
  width: 100%;
}

footer {
  display: flex;
  margin-left: 5%;
  margin-top: 1%;
}

footer h4 {
  margin: 0%;
}
</style>
