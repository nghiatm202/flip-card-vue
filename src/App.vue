<template>
  <MainScreen
    v-if="statusMatch === 'default'"
    @onStart="onHandleBeforeStart($event)"
  />
  <InteractiveScreen v-if="statusMatch === 'match'" />
</template>

<script>
import MainScreen from "./components/MainScreen.vue";
import InteractiveScreen from "./components/InteractiveScreen.vue";
export default {
  name: "App",
  data() {
    return {
      statusMatch: "default",
    };
  },
  components: {
    MainScreen,
    InteractiveScreen,
  },
  methods: {
    onHandleBeforeStart(totalOfBlock) {
      this.statusMatch = "match";
      console.log(totalOfBlock);
    },
  },
};
</script>
