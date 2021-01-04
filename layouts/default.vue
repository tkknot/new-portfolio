<template>
  <v-app>
    <headerComponent />

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <footerComponent />
  </v-app>
</template>

<script>
import headerComponent from "~/components/layouts/header";
import footerComponent from "~/components/layouts/footer";

export default {
  components: {
    headerComponent,
    footerComponent
  }
};
</script>
