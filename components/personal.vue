<template>
  <div class="mt-16">
    <h1 class="text-center">Personal Skill</h1>
    <v-container class="mt-12">
      <v-row>
        <v-col cols="3" class="mx-auto" v-for="(item, i) in items" :key="i">
          <v-card height="480">
            <v-img :src="item.src"></v-img>
            <h2 class="text-center  py-1">{{ item.h2 }}</h2>
            <v-card-text class="text-h6 jp">{{ item.text }}</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

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
  }
};
</script>
