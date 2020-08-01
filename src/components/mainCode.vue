<template>
  <div class="all">
    <!-- 标题 -->
    <h1>2048</h1>
    <!-- 新游戏 按钮 -->
    <button class="btn">new game</button>
    <!-- 分数统计 -->
    <h4>score: {{score}}</h4>
    <!-- 游戏区域 -->
    <div class="grid-contain">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>
</template>
<script>
export default {
  name: "mainCode",
  data() {
    return {
      score: 0
    };
  }
};
</script>
<style lang="less" scoped>
.all {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.btn {
  width: 200px;
  height: 60px;
  border: none;
  border-radius: 10px;
  line-height: 60px;
  color: white;
  background-color: #cc826c;
}
.grid-contain {
  width: 460px;
  height: 460px;
  padding: 20px;
  background-color: #bbada0;
  border-radius: 10px;
  display: grid;
  grid-template-columns: repeat(4, 100px);
  grid-template-rows: repeat(4, 100px);
  grid-row-gap: 20px;
  grid-column-gap: 20px;
  div {
    width: 100px;
    height: 100px;
    background-color: #ccc0b3;
    text-align: center;
    line-height: 100px;
    font-size: 40px;
  }
}
</style>>
