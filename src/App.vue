<template>
  <div>
    <ComponenteBoco 
      v-for="event in timeline" :key="event.title" 
      :title="event.title" 
      :content="event.content"
    ></ComponenteBoco>
        <nav> 
         <li><a href="">Home</a></li>
            <li><a href="">News</a></li>
            <li><a href="">Profile</a></li>
            <li><a href="">Biography</a></li>
            <li><a href="">Discography</a></li>
            <li><a href="">Schedule</a></li>
            <li><a href="">Contact</a></li>
            <li><a href="">Link</a></li>
        </nav> 
        <img src="banner.jpg">  

        <h2>Profile</h2>
        <img src="">

        <h2>Biography</h2>
        // deixar anotado https://night-child.net/psycho-sonic-boom


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

nav li {
  display: inline;
  margin: 0 0 0 15px;
}

</style>
