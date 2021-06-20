<template>
  <div class="container">
    <h1 class="title"><span id="view_time"></span>Todo List</h1>

    <a href="#" class="input_container">
      <input type="text" id="todos" class="todos" name="todos">
      <div class="plus_icon"></div>
    </a>
  </div>
</template>

<style lang="scss" scoped>
.container {
  height: 100vh;
  width: 100vw;
  text-align: center;
}

.title {
  padding-top: 30px;
}

.title {
  color:#fabe00;
}

.input_container {
  display: flex;
  justify-content: center;
  margin: 30px 0;
}

.todos {
  border: 1px solid #fabe00;
  height: 26px;
  width: 187px;
  padding: 4px 8px;
  font-size: 14px;
  color: #191300;
}

.plus_icon {
  position: relative;
  width: 26px;
  height: 26px;
  background: #fabe00;
  border: 1px solid #fabe00;
  border-left: 0px;
  transition: all 0.3s ease-out;

  &::before, &::after {
    position: absolute;
    top: 11px;
    left: 13px;
    content: '';
    display: inline-block;
    width: 14px;
    height: 14px;
    border-top: 2px solid #fff;
    transform: translateX(-50%);
  }

  &::after {
    top: 5px;
    left: 0px;
    transform: rotate(90deg);
  }


  &:hover {
    background: white;

    &::before, &::after {
      border-top: 2px solid #fabe00;
    }
  }
}
</style>

<script>
  var today = new Date();
  console.log(today)
</script>


