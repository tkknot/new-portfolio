<template>
  <div class="mt-14">
    <h1 class="text-center" id="a">Profile</h1>

    <v-container class="mt-12">
      <v-row>
        <v-col cols="12" xl="6" lg="6" md="6">
          <v-img
            src="/img/me.jpeg"
            id="photo-box"
            class="rounded-xl mx-auto"
          ></v-img>
        </v-col>
        <v-col cols="12" xl="6" lg="6" md="6">
          <p class="text-xl-h5 text-h7 jp">
            現在21歳、読書が好きだということをきっかけに、<br />
            世田谷の大学で文学を専攻している文系大学生です。
          </p>
          <p class="text-xl-h5 text-h7 jp">
            筋トレとライフハックが好きで、<br />自己管理能力には定評があります。
          </p>
          <p class="text-xl-h5 text-h7 jp">
            学生時代は2つの団体運営と6つの資格取得など、<br />複数活動に注力していました。
          </p>
          <p class="text-xl-h5 text-h7 jp">
            現在、フロントエンドの技術をメインに、<br />プログラミングを独学で勉強しています。
          </p>
          <p class="text-xl-h5 text-h7 jp">
            また、自分の知識や熱量で人の役に立ちたいという思いから、エンジニア職を見ています。
          </p>
        </v-col>
      </v-row>
    </v-container>
    
  </div>
</template>

<style lang="scss" scoped>
#photo-box {
  width: 80%;
  height: 84%;
}

@media screen and (min-width: 1000px) {
  .jp {
    font-size: 1.2rem;
  }
}
</style>
