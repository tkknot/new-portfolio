<template>
  <div class="mt-16">
    <h1 class="text-center" id="c">Personal Skill</h1>
    <v-container class="mt-12">
      <v-row>
        <v-col
          cols="4"
          xl="3"
          lg="3"
          md="3"
          sm="3"
          class="mx-auto"
          v-for="(item, i) in items"
          :key="i"
        >
          <v-card :height="height">
            <v-img :src="item.src" class="p-3"></v-img>
            <h2 class="text-center py-1 text-h5" id="item-title">
              {{ item.h2 }}
            </h2>
            <p class="text-xl-h5 text-h7 mt-3 px-3 jp">{{ item.text }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>
@media screen and (max-width: 480px) {
  .jp {
    font-size: 0.8rem !important;
  }
  #item-title {
    font-size: 1rem !important;
  }
}
</style>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "/img/study.svg",
          h2: "Qualification",
          text: "金融系から語学系まで、6つの資格を持っています。"
        },
        {
          src: "/img/macho.svg",
          h2: "Stoic",
          text:
            "食事管理とライフハックを日常的に行っているので、常にベストコンディションです。"
        },
        {
          src: "/img/canhoo.svg",
          h2: "Greedy",
          text: "好奇心旺盛で、やりたいと思ったことには果敢に取り組みます。"
        }
      ]
    };
  },
  computed: {
    height: function() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 320;
        case "sm":
          return 380;
        default:
          return 480;
          break;
      }
    }
  }
};
</script>
