<template>
  <div class="container">
    <AppHeader />
    <slot></slot>
    <div v-if="$device.isMobile">
      <MobileNavigator />
    </div>
  </div>
</template>

<script lang="js">
</script>

<style lang="scss">
html {
  font-size: 1rem;
  word-spacing: 1px;
  box-sizing: border-box;
}

html,
body,
#__nuxt,
#__layout,
.container {
  min-height: 100vh;
  width: 100%;
  margin: 0;
}

*,
*:before,
*:after {
  font-family: "Open Sans Bold";
}
</style>