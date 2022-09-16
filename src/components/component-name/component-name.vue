<template>
  <div class="component-name">
    <div class="component-name__header">
      <img src="./icon.svg" alt="Icon" class="component-name__img" />
      <span>{{ name }}</span>
    </div>
    <div class="component-name__time">
      时间：
      {{ new Date().getFullYear() }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'component-name',
  props: {
    name: {
      type: String,
      default: 'wytxer'
    }
  }
}
</script>

<style lang="less" scoped>
.component-name {
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  position: relative;
  width: 500px;
  height: 200px;
  padding: 10px;
  background-color: #f8f8f8;
  border-radius: 10px;
  margin-right: 16px;
  box-shadow: 2px 2px 8px #d9d9d9;
  &__header {
    font-size: 20px;
    color: #158dff;
    display: flex;
    align-items: center;
  }
  &__img {
    width: 24px;
    vertical-align: middle;
    margin-right: 10px;
  }
  &__time {
    position: absolute;
    bottom: 8px;
    right: 8px;
    color: #666;
    font-size: 12px;
  }
}
</style>
