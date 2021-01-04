<template>
  <div class="my-16">
    <h1 class="text-center" id="d">Portfolio</h1>
    <v-container class="mt-12">
      <v-carousel hide-delimiters>
        <v-carousel-item
          v-for="(photo, i) in photos"
          :src="photo.src"
          :key="i"
          nuxt
          transition="fade-transition"
        >
          <a :href="photo.link" id="link" class="white--text">
            <v-sheet tile :color="photo.color">
              <div class="display-2 text-h6 pl-3" id="link-box">
                <span>{{ photo.title }}</span>
              </div>
            </v-sheet>
          </a>
        </v-carousel-item>
      </v-carousel>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>
#link {
  text-decoration: none;
}

#link-box {
  &:hover {
    cursor: pointer;
    background: rgba(134, 227, 255, 0.705);
  }
}
</style>

<script>
export default {
  data() {
    return {
      photos: [
        {
          src: "/img/logo-new.jpeg",
          link: "https://kassa-yuu.com/",
          title: "kassa-yuu",
          color: "pink lighten-2"
        },
        {
          src: "/img/workout.jpeg",
          link: "https://self-train.com/",
          title: "Carories App",
          color: "yellow lighten-2"
        }
      ]
    };
  }
};
</script>
