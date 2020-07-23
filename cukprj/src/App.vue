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
      <v-tabs
      dark
      right
      v-model="tab"
      >
      <v-tab v-for="item in items" :key="item">{{item}}</v-tab>
      </v-tabs>
    </v-app-bar>

    <v-main>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center"> </v-row>
        <v-tabs-items v-model="tab">
          <v-tab-item></v-tab-item>
          <v-tab-item><product-page></product-page></v-tab-item>
          <v-tab-item><process-page></process-page></v-tab-item>
          <v-tab-item><market-analysis-page></market-analysis-page></v-tab-item>
      </v-tabs-items>
      </v-container>
    </v-main>
    <v-btn bottom color="pink" dark fab fixed right>
      <v-icon>mdi-plus</v-icon>
    </v-btn>
    
  </v-app>
</template>

<script>
import ProductPage from './components/Page/ProductPage.vue'
import ProcessPage from './components/Page/ProcessPage.vue'
import MarketAnalysisPage from './components/Page/MarketAnalysisPage.vue'

export default {
  name: 'mainPage',
  components: {
    ProductPage,
    ProcessPage,
    MarketAnalysisPage,
  },
  props: {
    source: String,
  },
  data: () => ({
    tab: null,
    items: ['Home', '제품소개', '제품원리', '시장분석'],
  }),
};
</script>
