<template>
<div>
  <!-- <img alt="Vue logo" src="./assets/logo.png" > -->
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <Header />
  <Arif data="icc wtc" cmp="Datamatics"/>
  <ConditionalRender/>
  <ForLoop />
  <ButtonClick />
  <classStyleBind />
  <DataBinding />
  <Form />
  <FetchApi />

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Arif from './components/Arif.vue'
import Header from './components/Header.vue'
import ConditionalRender from './components/ConditionalRender.vue'
import ForLoop from './components/ForLoop.vue'
import ButtonClick from './components/ButtonClick.vue'
import classStyleBind from './components/classStyleBind.vue'
import DataBinding from './components/DataBinding.vue'
import Form from './components/Form.vue'
import FetchApi from './components/FetchApi.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Header,
    Arif,
    ForLoop,
    ConditionalRender,
    ButtonClick,
    classStyleBind,
    DataBinding,
    Form,
    FetchApi
    
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


