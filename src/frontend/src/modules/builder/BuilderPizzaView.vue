<template>
  <div class="content__constructor">
    <div class="pizza pizza--foundation--big-tomato">
      <div
        class="pizza__wrapper"
        @drop="onDrop($event, 1)"
        @dragover.prevent
        @dragenter.prevent
      >
        <div class="pizza__filling pizza__filling--ananas"></div>
        <div class="pizza__filling pizza__filling--bacon"></div>
        <div class="pizza__filling pizza__filling--cheddar"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BuilderPizzaView",
  methods: {
    onDrop: function () {
      console.log("1");
    },
  },
};
</script>
