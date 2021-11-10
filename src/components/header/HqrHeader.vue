<template>
  <div class="header">
    <div>
      <span v-text="msg"></span>
      <span>logo</span>
    </div>

    <div>登录</div>
  </div>
</template>

<script>
export default {
  props: {
    msg: String,
  },
};
</script>

<style scope>
.header {
  display: flex;
  justify-content: space-between;
  height: 50px;
}
.header span:nth-child(1) {
  color: red;
  display: inline-block;
  margin-left: 10px;
}
</style>