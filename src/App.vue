<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div>
    <h4 class="red" :style = "스타일">XX 원룸</h4>
    <p>{{ price1 }} 만원</p>
  </div>
  <div>
    <h4>XX 원룸</h4>
    <p>{{ price2 }} 만원</p>
  </div>

</template>

<script>
//1. js 데이터를 HTML에 꽂아넣는 문법(데이터 바인딩)
//데이터 바인딩을 하는 이유1 - NTML에 하드 코딩을 해놓으면 나중에 변경하기 어려움
//데이터 바인딩을 하는 이유2 - 실시간 자동 렌더링을 쓰기 위해서 
//HTML 속성도 데이터바인딩 가능 - :속성="데이터 이름"으로 작성하면 됨

export default {
  name: 'App',
  //data 보관함
  data(){
    return {
      //여기서부터 데이터 보관하는 곳(변수 작성)
      //작성한 데이터를 HTML에 꽂아넣고 싶으면 {{데이터 이름}}으로 작성하면 됨.
      price1 : 60,
      price2 : 70,
      스타일 : 'color : blue',
      products : ['역삼동원룸', '천호동원룸', '마포구원룸'],
    }
  },
  components: {
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
