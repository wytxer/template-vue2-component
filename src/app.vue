<template>
  <div id="app" class="page-app">
    <header class="page-app__header">
      Template Vue Component
    </header>
    <div class="page-app__body">
      <router-view />
    </div>
  </div>
</template>

<style lang="less" scoped>
.page-app {
  &__header {
    color: #158dff;
    padding: 16px 32px;
    font-size: 24px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  &__body {
    padding: 16px 32px;
  }
}
</style>
