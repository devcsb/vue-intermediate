<template>
  <div id="app">
    <TodoHeader></TodoHeader> <!--PascalCase vs kebab-case 선택-->
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>
<todo
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

</style>
