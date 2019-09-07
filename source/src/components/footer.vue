<template>
  <a-layout-footer class="footer">
    <a-back-top />
      <a-button type="link">© 2019 <a-icon type="user" />鲍鹏</a-button>
    <a-button icon="mail" type="link">841244060@qq.com</a-button>


  </a-layout-footer>
</template>
<script>
export default {};
</script>
<style lang="scss">
.footer.ant-layout-footer {
  height: 100%;
  background: #101010;
  text-align: center;
  padding: 10px;
  button {
    font-size: 1.1em;
    color: #9d9d9d;
    &:hover {
      color: #fff;
      cursor: pointer;
    }
  }
}
</style>