<template>
  <div class="box">
    <div class="position">
      <dl>
        <dt class="mark">
          <img src="../assets/mark.png" alt>
        </dt>
        <dd>请先完善资料，再进行下一步操作</dd>
      </dl>
      <button class="button">确认</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
<style>
.box {
  width: 100%;
  height: 100%;
  position: absolute;
  background-color: #ebebeb;
}
.position{
  position: relative;
  top: 35%;
}
.mark {
  margin-bottom: 0.5rem;
}
dl > dd {
  margin-bottom: 0.5rem;
  font-size: 14px;
  font-weight: 500;
}
.mark img {
  width: 3rem;
  height: 3rem;
}
.button {
  width: 8.5rem;
  height: 1rem;
  color: #fff;
  background-color: #00b24c;
  border-color: #00b24c;
  display: inline-block;
  line-height: 1;
  white-space: nowrap;
  cursor: pointer;
  border: 1px solid #dcdfe6;
  -webkit-appearance: none;
  text-align: center;
  box-sizing: border-box;
  outline: none;
  margin: 0;
  transition: 0.1s;
  font-weight: 500;
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
  padding: 12px 20px;
  font-size: 14px;
  border-radius: 4px;
}
</style>
