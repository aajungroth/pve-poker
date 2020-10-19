<template>
  <div class="action-box">
    <h1>
      Actions
    </h1>
    <button>
      Check
    </button>
    <button>
      Bet
    </button>
    <button>
      Call
    </button>
    <label>
      Raise Amount
    </label>
    <input type="number" min="0" max="1000000"/>
    <button>
      Rasie
    </button>
    <button>
      Rerasie
    </button>
    <button>
      Fold
    </button>
  </div>
</template>

<script>
export default {
  name: 'ActionPanel',
  props: {},
  data() {
    return {};
  },
  methods: {}
}
</script>

<style scoped>
  .action-box {
    border-color: #0000FF;
    border-style: solid;
    display: flex;
    flex-direction: column;
  }
</style>
