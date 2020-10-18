<template>
  <div class="chat-box">
    <h1>Chat Log</h1>

    <ul>
      <li v-for="(message, index) in messageList" :key="index">
        {{ message.text }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ChatLog',
  props: {},
  data() {
    return {
      messageList: [
        {
          id: 1,
          text: 'This is a test.'
        },
        {
          id: 2,
          text: 'Stuff happened.'
        },
        {
          id: 3,
          text: 'A player had the most successful simulation.'
        }
      ]
    };
  },
  methods: {}
}
</script>

<style scoped>
  .chat-box {
    border-color: #FF0000;
    border-style: solid;
  }
</style>
