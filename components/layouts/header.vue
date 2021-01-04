<template>
  <div>
  <v-app-bar app height="500" src="/img/home.jpg" absolute>
  <v-container class="mt-auto">
  <p id="title" class="text-right">TK's Portfolio</p>
    <v-row class="m-0">
      <v-col v-for="(e, i) in elements" :key="i" cols="3" class="text-center" id="menu">
        <a class="d-block" id="anker">
        <!-- <a class="white--text" v-for="(link, i) in links" :href="link[i]"> -->
        {{e.sentence}}
        </a>
        </v-col>
    </v-row>
  </v-container>
  </v-app-bar>
  </div>
</template>

<style lang="scss" scoped>
#title {
  color: white;
  font-size: 4rem;
  width: 100%;
  height: 150px;
  margin-bottom: 180px;
}

  #anker {
    width: 100%;
    height: 100%;
    color: white;
    font-size: 1.2rem;
  }

  #menu {
    &:hover {
      background-color: rgba(255,255,255,0.4);
      cursor: pointer;
      & > a {
        color: black;
      }
    }
  }
</style>

<script>
export default {
  data(){
  return{
    elements: [
      {sentence: 'Profile'},
      {sentence: 'Programming Skill'},
      {sentence: 'Personal Skill'},
      {sentence: 'PortFolio'},
    ],
    // links: [
    //   {link: '#a'},
    //   {link: '#b'},
    //   {link: '#c'},
    //   {link: '#d'},
    // ]
  }
  }
}
</script>