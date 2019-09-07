<template>
  <a-layout-content class="content">
    <my-item></my-item>
  </a-layout-content>
</template>
<script>
import item from "./item";
export default {
  components: {
    "my-item": item
  }
};
</script>
<style lang="scss">
.content {
  display: flex;
  justify-content: space-around;
  text-align: center;
}
</style>