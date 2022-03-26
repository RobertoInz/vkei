<template>
  <div>
    <ComponenteBoco 
      v-for="event in timeline" :key="event.title" 
      :title="event.title" 
      :content="event.content"
    ></ComponenteBoco>
  </div>
</template>

<script>

import ComponenteBoco from "./components/ComponenteBoco";

export default {
  name: 'App',
  components: {
    ComponenteBoco
  },
  data() {
    return {
      timeline: [
        {
          title: "Início em 1980",
          content: "Aqui começa a putaria"
        },
        {
          title: "Início em 1981",
          content: "Aqui continua a putaria"
        },
        {
          title: "Início em 1982",
          content: "Aqui morre a putaria"
        },
        {
          title: "Início em 1983",
          content: "Aqui volta a putaria"
        },
      ]
    }
  }
}
</script>

<style>
</style>
