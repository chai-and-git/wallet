<template>
  <div class="nav-list">
    <ul>
      <li>
        <NuxtLink to="/">
          <img src="/images/home-nav-mobile.png" class="nav-image">
          <span>Home</span>
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/cards">
          <img src="/images/cards-nav-mobile.png" class="nav-image">
          <span>Cards</span>
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/payments">
          <img src="/images/payments-nav-mobile.png" class="nav-image">
          <span>Payments</span>
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/credit">
          <img src="/images/credit-nav-mobile.png" class="nav-image">
          <span>Credit</span>
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/profile">
          <img src="/images/profile-nav-mobile.png" class="nav-image">
          <span>Profile</span>
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>

<style lang="scss">
.nav-list {
  //filter: drop-shadow(0 -3px #00000014);
  -webkit-box-shadow: -1px -3px 2px #00000014;
  -moz-box-shadow: -1px -3px 2px #00000014;
  box-shadow: -1px -3px 2px #00000014;
}

.nav-list {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: auto;

  ul {
    list-style: none;
    display: contents;
    

    li {
      float: left;
      width: 20%;
      vertical-align: top;
      display: inline;
      text-align: center;
      box-sizing: border-box;
      padding: 5px;

      a {
        text-decoration: none;
      }

      a:link, a:visited {
        color: #DDDDDD;
      }

      span {
        display: block;
        position: relative;
        font-size: 13px;
        bottom: 0;
      }

      .nav-image {
        height: 24px;
      }
    }
  }
}
</style>