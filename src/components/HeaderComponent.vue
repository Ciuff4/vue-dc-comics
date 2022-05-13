<template>
  <header class="container">
      <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
          <ul>
              <li><a href="#">CHARACTERS</a></li>
              <li><a class="active" href="#">COMICS</a></li>
              <li><a href="#">MOVIES</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">GAMES</a></li>
              <li><a href="#">COLLECTIBLES</a></li>
              <li><a href="#">VIDEOS</a></li>
              <li><a href="#">FANS</a></li>
              <li><a href="#">NEWS</a></li>
              <li><a href="#">SHOP</a></li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
name:'HeaderComponent'
}
</script>

<style lang="scss" scoped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
        .logo{
            width: 70px;
        }
        ul{
            display: flex;
            justify-content: space-around;
            list-style: none;
            li{
                a{
                    display: inline-block;
                    text-decoration: none;
                    font-weight: bold;
                    color:#434344;
                    padding: 0 5px;
                    height: 80px;
                    &:hover{
                        color: #0E88F9;
                    };
                    &.active{
                        color: #0E88F9;
                    }
                }
            }
        }
    }
</style>