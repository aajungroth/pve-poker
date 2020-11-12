<template>
  <div class="main-panel">

    <ChatLog/>

    <div class="game-panel">

      <div class="inner-panel">
        <SimulationView/>
        <ActionPanel/>
      </div>

      <GoldView/>

    </div>

  </div>

  <img alt="Vue logo" src="./assets/logo.png">

  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import ActionPanel from './components/ActionPanel.vue';
import ChatLog from './components/ChatLog.vue';
import GoldView from './components/GoldView.vue';
import HelloWorld from './components/HelloWorld.vue';
import SimulationView from './components/SimulationView.vue';

export default {
  name: 'App',
  components: {
    ActionPanel,
    ChatLog,
    GoldView,
    HelloWorld,
    SimulationView
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

.main-panel {
  display: flex;
  flex-direction: row;
}

.game-panel {
  display: flex;
  flex-direction: column;
}

.inner-panel {
  display: flex;
  flex-direction: row;
  flex-grow: 0;
  flex-shrink: 0;
  flex-basis: 100%;
}
</style>
