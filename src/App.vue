<template>
  <div id="app">
    <header>
      <img src="./assets/logo.png">
      <nav>
        <ul>
          <li><router-link :to="{ name: 'Create' }">Create</router-link></li>
          <li><router-link :to="{ name: 'Preview' }">Preview</router-link></li>
        </ul>
      </nav>
    </header>
    <main>
      <router-view/>
    </main>
    <footer>
      <p>made by <span>userJapa</span></p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
@import 'assets/sass/main.scss';

#app {
  height: 100%;
  display: grid;
  grid-template-rows: 1fr 4fr .5fr;
  header {
    display: flex;
    justify-content: center;
    flex-direction: column;
    img, nav {
      align-self: center;
      display: inline-block;
    }
    img {
      width: 12.5%;
      height: auto;
    }
    nav {
      text-align: center;
      ul {
        list-style: none;
        li {
          font-size: 2rem;
          display: inline;
          a {
            text-decoration: none;
            color: $color-black;
            &:first-child { margin-left: 10px; }
          }
        }
      }
    }
  }
  footer {
    font-size: 2rem;
    display: flex;
    justify-content: flex-end;
    p {
      align-self: flex-end;
      display: inline;
    }
  }
}

</style>
