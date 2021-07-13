<template>
  <header class="container">
    <nav>
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="Logo DC" />
      </div>

      <div class="menu">
        <ul>
          <li><a href="">CHARACTERS</a></li>
          <li><a href="">COMICS</a></li>
          <li><a href="">MOVIES</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">GAMES</a></li>
          <li><a href="">COLLECTIBLES</a></li>
          <li><a href="">VIDEOS</a></li>
          <li><a href="">FANS</a></li>
          <li><a href="">NEWS</a></li>
          <li><a href="">SHOP</a></li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data: function() {
    //TODO: stampare il menu dinamicamente dai data
    /* menuLinks: [
      {
        href: '#',
        name: 'CHARACTERS',
      },
      {},
      {},
    ]; */
  },
};
</script>

<style scoped lang="scss">
@import '../style/colors';

header {
  height: 80px;
  padding: 10px 0;

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
      height: 60px;
    }

    ul {
      display: flex;

      li {
        a {
          color: black;
          font-family: 'Roboto Condensed', sans-serif;
          font-weight: bold;
          margin-left: 24px;
          padding-bottom: 23px;

          &:hover {
            color: $dc-blue-color;
            border-bottom: 5px solid $dc-blue-color;
          }
        }
      }
    }
  }
}
</style>
