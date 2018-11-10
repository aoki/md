<template>
  <div id="layout-container">
    <div id="drag-space"></div>
    <nuxt/>
  </div>
</template>

<style>
  #layout-container {
    width: inherit;
    height: inherit;
    display: flex;
    flex-direction: column;
  }
  #drag-space {
    -webkit-app-region: drag;
    flex-basis: 24px;
  }
</style>
