<template>
  <div>
    <v-app-bar app height="500" src="/img/home.jpeg" absolute>
      <v-container class="mt-auto">
        <p id="title" class="text-right">TK's Portfolio</p>
        <v-row class="m-0">
          <v-col
            v-for="(e, i) in elements"
            :key="i"
            cols="3"
            class="text-center"
            id="menu"
          >
            <a class="d-block text-h6" id="anker" :href="e.link">
              <span>
                {{ e.sentence }}
              </span>
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
  font-family: "Noto Sans", sans-serif;
}

#anker {
  width: 100%;
  height: 100%;
  color: white;
  font-size: 1.2rem;
  text-decoration: none;
}

#menu {
  &:hover {
    background-color: rgba(255, 255, 255, 0.4);
    cursor: pointer;
    & > a {
      color: black;
    }
  }
}

@media screen and (min-width: 600px) {
  #anker {
    font-size: 1rem !important;
  }
}

@media screen and (min-width: 300px) {
  #anker {
    font-size: 0.8rem !important;
  }
}
</style>

<script>
export default {
  data() {
    return {
      elements: [
        { sentence: "Profile", link: "#a" },
        { sentence: "Programming Skill", link: "#b" },
        { sentence: "Personal Skill", link: "#c" },
        { sentence: "PortFolio", link: "#d" }
      ]
    };
  }
};
</script>
