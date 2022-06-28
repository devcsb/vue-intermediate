<template>
  <div id="app">
    <TodoHeader></TodoHeader> <!--PascalCase vs kebab-case 선택-->
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>

  </div>
</template>

<script>
import TodoHeader from "./components/TodoHeader";
import TodoInput from "./components/TodoInput";
import TodoList from "./components/TodoList";
import TodoFooter from "./components/TodoFooter";

// // es5의 방식
// var my_cmp = {
//   template: '<div>my component</div>'
// };
//
// new Vue({
//   el: '',
//   components: {
//     // '컴포넌트 이름': '컴포넌트 내용'
//     'my-cmp': my_cmp
//   }
// })
export default {
  components: {
    // 컴포넌트 태그 명 : 컴포넌트 내용
    'TodoHeader': TodoHeader,
    'TodoInput' : TodoInput,
    'TodoList' : TodoList,
    'TodoFooter' : TodoFooter,

  }

}
</script>

<style>
body{
  text-align: center;
  background-color: #F6F6F6;
}
input {
  border-style: groove;
}
button{
  border-style: groove;
}
.shadow{ /* 그림자 효과 */
  box-shadow: 5px 10px 10px rgba(0,0,0, 0.03);
}

</style>
