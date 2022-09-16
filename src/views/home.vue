<template>
  <div class="page-home">
    <layout-box title="Card" description="基于业务定制的卡片容器。">
      <component-name />
    </layout-box>
    <layout-box title="Card" description="打完包后的效果">
      <lib-component-name />
    </layout-box>
  </div>
</template>

<script>
import { ComponentName as LibComponentName } from '../../lib/component-name.umd.min'

export default {
  components: {
    LibComponentName
  }
}
</script>
