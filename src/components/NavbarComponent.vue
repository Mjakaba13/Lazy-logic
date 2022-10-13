<template>
  <nav>
    <div class="nav-content">
      <div class="logo">
        <img src="../assets/logo.svg" alt="company logo" />
      </div>
      <ul>
        <li><router-link :to="{ name: 'home' }">Home</router-link></li>
        <li><router-link :to="{ name: 'home' }">What we do</router-link></li>
        <li><router-link :to="{ name: 'home' }">About</router-link></li>
        <li><router-link :to="{ name: 'home' }">Contact Us</router-link></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
nav {
  background: #000000;
  display: flex;
  justify-content: center;
  align-items: center;
  .nav-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    // padding: 16px 249px;
    width: calc(100% - 48px);
    max-width: 853px;

    .logo {
      img {
        width: 100%;
        height: 100%;
      }
    }
  }

  ul {
    display: none;
  }
  li {
    list-style: none;
    margin-left: 13px;
  }
  a {
    text-decoration: none;
    font-family: "Inter";
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    display: flex;
    align-items: center;
    text-align: center;
    color: #ffffff;
  }
  @media (min-width: 768px) {
    ul {
      display: flex;
    }
  }
}
</style>
