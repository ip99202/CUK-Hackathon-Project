<template>
  <v-app id="inspire">
    <v-app-bar
      :clipped-left="$vuetify.breakpoint.lgAndUp"
      app
      color="grey darken-1"
      dark
    >
      <v-toolbar-title style="width: 300px" class="ml-0 pl-4">
        <span class="hidden-sm-and-down">어울림</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <v-tabs dark right v-model="tab">
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
          <v-tabs-items v-model="tab">
            <v-tab-item></v-tab-item>
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
