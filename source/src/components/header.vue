<template>
    <a-layout-header class="header">
      <div class="nav-btn">
        <a-button type="link" icon="bars" @click="show ? show = false : show = true"></a-button>
      </div>
      <ul :class="{hidden : show}" class="nav-scroll">
        <li>
          <a-button icon="home" type="link">主页</a-button>
        </li>
        <li>
          <a-button icon="book" type="link">练习demo</a-button>
        </li>
        <li>
          <a href="https://github.com/BP-baopeng" target="_black">
            <a-button icon="github" type="link">GitHub</a-button>
          </a>
        </li>
        <li>
          <a href="https://bp-baopeng.github.io/" target="_black">
            <a-button icon="cloud" type="link">个人博客</a-button>
          </a>
        </li>
        <li>
          <a href="javascript:;" target="_black">
            <a-button icon="link" type="link">关于</a-button>
          </a>
        </li>
      </ul>
    </a-layout-header>
</template>
<script>
export default {
  data() {
    return {
      show: true
    };
  }
};
</script>
<style lang="scss">
.header.ant-layout-header {
  background-color: #333;
  height: 100%;
  .nav-btn {
    display: none;
    height: 100%;
    > button {
      height: 100%;
      width: 60px;
      font-size: 2em;
      color: #9d9d9d;
    }
  }
  .nav-scroll {
    border-top: 1px solid #101010;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: flex-end;
    padding: 10px 0;
    margin: 0;
    li {
      height: 100%;
      line-height: 0;
    }
  }
  button {
    font-size: 1.1em;
    color: #9d9d9d;
    &:hover {
      color: #fff;
      cursor: pointer;
    }
  }
}
@media screen and (max-width: 768px) {
  .header.ant-layout-header {
    z-index: 999;
    height: 100%;
    padding: 0 10px;
    .nav-scroll.hidden {
      display: none;
    }
    .nav-btn {
      display: block;
      height: 53px;
    }
    .nav-scroll {
      display: flex;
      flex-direction: wrap;
      flex-wrap: wrap;
      background: #333;
      padding: 10px 0;
      li {
        width: 100vw;
        height: 35px;
      }
    }
    button {
      text-align: left;
      font-size: 0.9em;
      color: #9d9d9d;
      width: 100%;
      &:hover {
        color: #fff;
      }
    }
  }
}
</style>