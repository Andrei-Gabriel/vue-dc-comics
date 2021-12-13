<template>
  <header>
      <div class="header-container">
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
      </div>
  </header>
</template>

<script>
    export default {
        name: 'Header',
    }
</script>

<style lang="scss" scoped>
    // Importato per poter usare @mixin e quindi @include
    @import '../assets/style/global.scss';
    header {
        .header-container{
            @include width-content;
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
    }
</style>