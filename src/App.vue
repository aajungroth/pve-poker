<template>
  <img alt="Vue logo" src="./assets/logo.png">

  <div class="main-panel">

    <ChatLog/>

    <div class="game-panel">

      <div class="inner-panel">
        <div>Simulation View</div>
        <ActionPanel/>
      </div>

      <div>Gold View</div>

    </div>

  </div>

  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import ActionPanel from './components/ActionPanel.vue';
import ChatLog from './components/ChatLog.vue';
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    ActionPanel,
    ChatLog,
    HelloWorld
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

.main-panel{
  display: flex;
  flex-direction: row;
}

.game-panel{
  display: flex;
  flex-direction: column;
}

.inner-panel{
  display: flex;
  flex-direction: row;
}
</style>
