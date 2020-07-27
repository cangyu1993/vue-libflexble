<template>
  <div>
    <van-button type="primary">主要按钮</van-button>
    <van-button type="warning" size="large">大号按钮</van-button>
    <div class="needWidths"></div>
  </div>
</template>
<script>
export default {
  name: "HelloWorld"
};
</script>
<style>
.mu-demo-form {
  width: 100%;
  max-width: 750px;
}
.needWidths {
  width: 750px;
  height: 250px;
  background-color: red;
}
</style>
