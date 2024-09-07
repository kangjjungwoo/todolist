<script setup>
import HelloWorld from './components/HelloWorld.vue'
import {ref} from 'vue';

const inputValue = ref('');
const todoList = ref([]);

console.log(todoList.value);

const handleChange = (event) =.{
  const nextValue = event.target.value;
  inputValue.value = nextValue;
}

const handleClickButton = () =>{
  const nextValue = e
};

const handleChange = (event) => {
  console.log(event)
  const nextValue = event.target.value;
  inputValue.Value = nextValue
};

// java 스크립트가 동적으로 제어하는 부분
</script>

<template>
  <h4>TODO LIST</h4>
  
  <input :model="inputValue">
  <!-- @change="handleChange" /> -->
  <p>{{ inputValue }}</p>
  

  
  
  <input v-model="inputValue"/>
  <button>확인</button>

  <div>
    <div>코드짜기</div>
    <button>삭제</button>
  </div>
<!-- cmd+/로 주석가능,, 그리고 여기까지는 Html 부분 -->
</template>

<!-- css -->
<style scoped>
.todo-item{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  border: 1px solid gray;
}
</style>
