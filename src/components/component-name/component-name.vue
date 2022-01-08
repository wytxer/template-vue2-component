<template>
  <div class="component-name-wrap">
    <div class="name">
      <img src="./icon.svg" alt="Icon" />
      <span>{{ name }}</span>
    </div>
    <div class="time">
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
.component-name-wrap {
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

  .name {
    font-size: 20px;
    color: #158dff;
    display: flex;
    align-items: center;
    img {
      width: 24px;
      vertical-align: middle;
      margin-right: 10px;
    }
  }
  .time {
    position: absolute;
    bottom: 8px;
    right: 8px;
    color: #666;
    font-size: 12px;
  }
}
</style>
