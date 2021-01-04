<template>
  <div class="mt-16">
    <h1 class="text-center">Programming</h1>
    <v-container class="mt-12">
      <v-row>
        <v-col cols="6">
          <v-col v-for="(s, i) in skillSet" :key="i" cols="12">
            <v-container>
              <v-row class="red lighten-5 ">
                <v-col cols="3" class="red lighten-2 text-center white--text">{{
                  s.language
                }}</v-col>
                <v-col cols="7" id="gage"
                  ><p class="red darken-1 gage-stick" :id="s.language"></p
                ></v-col>
                <v-col cols="2" class="text-center grey--text">{{
                  s.level + "%"
                }}</v-col>
              </v-row>
            </v-container>
          </v-col>
        </v-col>
        <v-col cols="6">
          <v-col v-for="(f, i) in frameSet" :key="i" cols="12">
            <v-container>
              <v-row class="blue lighten-5 ">
                <v-col
                  cols="3"
                  class="blue lighten-2 text-center white--text"
                  >{{ f.frameName }}</v-col
                >
                <v-col cols="7" id="gage"
                  ><p class="blue darken-1 gage-stick" :id="f.frameName"></p
                ></v-col>
                <v-col cols="2" class="text-center grey--text">{{
                  f.level + "%"
                }}</v-col>
              </v-row>
            </v-container>
          </v-col>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>
#gage {
  padding: 0;
}

.gage-stick {
  height: 100%;
  margin: 0;
}

#Responsive,
#Bootstrap {
  width: 80%;
}
#JavaScript,
#Vuetify {
  width: 70%;
}
#HTML,
#CSS,
#Vue,
#Nuxt {
  width: 60%;
}
#SCSS {
  width: 30%;
}
#Python {
  width: 10%;
}
#Django {
  width: 20%;
}
#JQuery {
  width: 50%;
}
</style>

<script>
export default {
  data() {
    return {
      skillSet: [
        {
          language: "Responsive",
          level: "80"
        },
        {
          language: "JavaScript",
          level: "70"
        },
        {
          language: "HTML",
          level: "60"
        },
        {
          language: "CSS",
          level: "60"
        },
        {
          language: "SCSS",
          level: "30"
        },
        {
          language: "Python",
          level: "10"
        }
      ],
      frameSet: [
        {
          frameName: "Django",
          level: "20"
        },
        {
          frameName: "JQuery",
          level: "50"
        },
        {
          frameName: "Vue",
          level: "60"
        },
        {
          frameName: "Nuxt",
          level: "60"
        },
        {
          frameName: "Vuetify",
          level: "70"
        },
        {
          frameName: "Bootstrap",
          level: "80"
        }
      ]
    };
  }
};
</script>
