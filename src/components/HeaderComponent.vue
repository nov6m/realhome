<template>
  <nav class="navbar navbar-expand-lg navbar-light ">
  <div class="container">
    <a class="navbar-brand logo" href="/"><img src="../assets/images/logo/logo.png" alt="logo"></a>
    <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item menu-link" v-for="(menu, index) in headerMenuList" :key="index">
          <router-link class="nav-link active" aria-current="page" :to="menu.path">
            {{menu.name}}
          </router-link>
        </li>
      </ul>
      <div class="icons">
        <a href="https://www.facebook.com/" target="blank"><img src="../assets/images/icons/f.png" alt=""></a>
        <a href="https://www.pinterest.ru/" target="blank"><img src="../assets/images/icons/p.png" alt=""></a>
        <a href="https://www.instagram.com/" target="blank"><img src="../assets/images/icons/instagram.png" alt=""></a>
        <a href="https://www.google.ru/" target="blank"><img src="../assets/images/icons/g+.png" alt=""></a>
      </div>
    </div>
  </div>
</nav>
</template>

<script>
import {menuList} from '../constants/menuLinks';
export default {
  data(){
    return {
      headerMenuList: menuList,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/layouts/index';
.navbar {
  height: 90px;
}
.navbar-nav {
  height: 90px;
}
.logo {
  padding-right: 180px;
}
.collapse-fontsize {
  font-size: 18px;
}
.menu-link {
  padding: 25px 30px;
  &:hover {
  background: $greyLight;
  }
}
.icons {
  a {
    width: 30px;
    height: 30px;
    text-align: center;
    border: 1px solid $greyLight;
    border-radius: 15px;
    margin-right: 10px;
    display: inline-block;
  }
}

</style>
