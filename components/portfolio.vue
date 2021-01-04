<template>
  <div class="my-16">
    <h1 class="text-center">Portfolio</h1>
    <v-container class="mt-12">
      <v-carousel hide-delimiters>
        <v-carousel-item
          v-for="(photo, i) in photos"
          :src="photo.src"
          :key="i"
          nuxt
          :to="photo.link"
          transition="fade-transition"
        >
          <v-sheet tile :color="photo.color">
            <div class="display-2 text-h6 pl-3">
              {{ photo.title }}
            </div>
          </v-sheet>
        </v-carousel-item>
      </v-carousel>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      photos: [
        {
          src: "/img/logo-new.jpeg",
          link: "",
          title: "kassa-yuu",
          color: "pink lighten-2"
        },
        {
          src: "/img/workout.jpg",
          link: "",
          title: "Carories App",
          color: "yellow lighten-2"
        }
      ]
    };
  }
};
</script>
