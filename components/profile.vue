<template>
  <div class="mt-14">
    <h1 class="text-center">Profile</h1>
    <v-container class="mt-12">
      <v-row>
        <v-col cols="6">
          <div id="photo-box" class="rounded-xl">
            <v-img width="100%" height="100%" src=""></v-img>
          </div>
        </v-col>
        <v-col cols="6">
          <p class="text-h6">現在21歳、読書が好きだということをきっかけに、<br>
          世田谷の大学で文学を専攻している文系大学生です。</p>
          <p class="text-h6">筋トレとライフハックが好きで、<br>自己管理能力には定評があります。</p>
          <p class="text-h6">学生時代は2つの団体運営と6つの資格取得など、<br>複数活動に注力していました。</p>
            <p class="text-h6">現在、フロントエンドの技術をメインに、<br>プログラミングを独学で勉強しています。</p>
          <p class="text-h6">また、自分の知識や熱量で人の役に立ちたいという思いから、<br>エンジニア職を見ています。</p>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss">
  #photo-box {
    width: 200px;
    height: 200px;
  }
</style>