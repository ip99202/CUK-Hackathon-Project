<template>
  <v-container>
    <v-card class="mx-auto" flat>
      <v-container>
        <v-row justify="space-between">
          <v-col cols="auto">
            <v-img
              height="350"
              width="350"
              src="https://cdn.vuetifyjs.com/images/cards/store.jpg"
            ></v-img>
          </v-col>
          <v-col>
            <v-card-title>어울림이란</v-card-title>

            <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>

            <v-card-text class="text--primary">
              <div>Whitehaven Beach</div>

              <div>Whitsunday Island, Whitsunday Islands</div>
            </v-card-text>

            <v-card-actions>
              <v-btn color="orange" text>
                Share
              </v-btn>

              <v-btn color="orange" text>
                Explore
              </v-btn>
            </v-card-actions>
          </v-col>
        </v-row>
        <v-row justify="space-between">
          <v-col cols="auto">
            <v-img
              height="auto"
              width="600"
              src="https://user-images.githubusercontent.com/52627952/88538850-0f894380-d04b-11ea-949a-a1a908828378.jpg"
            ></v-img>
            출처 - 환경부 환경통계 포털
          </v-col>
          <v-col>
            <br>
            <v-card-title>어울림이란</v-card-title>

            <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>

            <v-card-text class="text--primary">
              <div>Whitehaven Beach</div>

              <div>Whitsunday Island, Whitsunday Islands</div>
            </v-card-text>

            <v-card-actions>
              <v-btn color="orange" text>
                Share
              </v-btn>

              <v-btn color="orange" text>
                Explore
              </v-btn>
            </v-card-actions>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: "ProductPage",

  data: () => ({}),
};
</script>
