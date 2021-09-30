<template>
  <div class="contanier">
    <column-list :list="list"></column-list>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
// import 'bootstrap/dist/css/bootstrap/min.css';
import ColumnList, { ColumnProps } from './components/ColumnList.vue'
const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'test1的专栏',
    description: '这是test1的专栏',
    avatar: ' https://cn.vitejs.dev/logo.svg'
  },
  {
    id: 1,
    title: 'test1的专栏',
    description: '这是test1的专栏',
    avatar: ' https://cn.vitejs.dev/logo.svg'
  }
]
export default defineComponent({
  name: 'App',
  components: {
    ColumnList
  },
  setup () {
    return {
      list: testData
    }
  }
})
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
