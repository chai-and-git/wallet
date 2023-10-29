<template>
  <div class="app-header">
    <img v-if="$device.isDesktop" src="/images/desktop-logo.png" class="logo" alt="aspire-logo" />
    <img v-else src="/images/mobile-logo.png" class="logo" alt="aspire-logo" />
  </div>
</template>

<script lang="js">
</script>

<style lang="scss" scoped>
.app-header {
  width: 100vw;
  height: 45px;
  padding: 15px;
  background-color: #0C365A;
  position: fixed;
  color: white;
  box-sizing: border-box;

  @media (min-width: 577px) {
    width: 20vw;
    height: 100%;
    padding: 40px;
  }

  .logo {
    float: right;
    
    @media (min-width: 577px) {
      float: left;
    }
  }
}
</style>