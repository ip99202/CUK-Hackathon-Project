<template>
  <v-app id="inspire">
    <v-app-bar :clipped-left="$vuetify.breakpoint.lgAndUp" app color="white">
      <v-toolbar-title class="ml-0 pl-4">
        <v-img
          class="center"
          height="55px"
          width="71.6375px"
          src="https://user-images.githubusercontent.com/54254402/88758978-b0d7dd00-d1a4-11ea-9991-fa651eef6569.png"
        ></v-img>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <v-tabs color="black" right v-model="tab">
        <v-tab v-for="item in items" :key="item">{{ item }}</v-tab>
      </v-tabs>
    </v-app-bar>

    <v-main>
      <v-lazy
        v-model="isActive"
        :options="{
          threshold: 0.5,
        }"
        min-height="200"
        transition="fade-transition"
      >
        <v-container fluid>
          <v-row align="center" justify="center"> </v-row>
          <v-tabs-items v-model="tab" class="v-flex justify-center mb-6">
            <v-tab-item
              ><v-card>
                <v-img

                  class="white--text align-start"
                  src="https://user-images.githubusercontent.com/52627952/88927184-0221c280-d2b2-11ea-93e9-5fcc6c436987.jpg"
                >
                  <div class="slogan">조용함을</div>
                  <div class="slogan">밝히다.</div></v-img
                ></v-card
              >
            </v-tab-item>
            <v-tab-item><product-page></product-page></v-tab-item>
            <v-tab-item><process-page></process-page></v-tab-item>
            <v-tab-item
              ><market-analysis-page></market-analysis-page
            ></v-tab-item>
          </v-tabs-items>
        </v-container>
      </v-lazy>
    </v-main>
    <back-to-top bottom="50px" right="50px">
      <v-btn color="primary" fab big dark>
        <v-icon>mdi-arrow-up-bold</v-icon>
      </v-btn>
    </back-to-top>
    <v-footer>
      <v-spacer></v-spacer>
      <div>
        &copy; POSTCORONA : 극도로 한정된 세계 極限 | 어울림 (한장희 박수환
        김지윤 허은지) {{ new Date().getFullYear() }}
      </div>
    </v-footer>
  </v-app>
</template>

<script>
import ProductPage from "./components/Page/ProductPage.vue";
import ProcessPage from "./components/Page/ProcessPage.vue";
import MarketAnalysisPage from "./components/Page/MarketAnalysisPage.vue";
import BackToTop from "vue-backtotop";

export default {
  name: "mainPage",
  components: {
    ProductPage,
    ProcessPage,
    MarketAnalysisPage,
    BackToTop,
  },
  props: {
    source: String,
  },
  data: () => ({
    tab: null,
    items: ["Home", "제품소개", "제품원리", "시장분석"],
    isActive: false,
  }),
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Nanum+Myeongjo:wght@400;700&display=swap");
.slogan {
  font-family: "Nanum Myeongjo", serif;
  font-size: 80px;
  margin-left: 50px;
  margin-top: 20px;
}
</style>
