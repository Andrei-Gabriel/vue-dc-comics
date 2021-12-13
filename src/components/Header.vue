<template>
  <header>
      <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="logo">
      </div>
      <nav class="header-nav">
          <ul>
              <li><a id="active" href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
              <li><a href="#">prova</a></li>
          </ul>
      </nav>
  </header>
</template>

<script>
    export default {
        name: 'Header',
    }
</script>

<style lang="scss" scoped>
    header {
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0 20px;
        // Logo
        .logo {
            img {
                height: 70px;
            }
        }
        .header-nav{
            width: 55%;
            // Lista di links .header-nav
            ul {
                display: flex;
                justify-content: space-between;
                // List item
                li {
                    list-style: none;
                    // Link
                    a {
                        display: inline-block;
                        line-height: 100px;
                        text-transform: uppercase;
                        text-decoration: none;
                        color: black;
                    }
                }
            }
        }
    }
</style>