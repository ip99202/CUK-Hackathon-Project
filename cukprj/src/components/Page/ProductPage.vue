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
        </v-row>

        <v-row>
          <v-col>
            <hr />
            <br />
            <v-card-subtitle class="pb-0"
              >저희 팀명이 가진 의미는 무엇일까요?</v-card-subtitle
            >
            <v-card class="d-inline-block mx-auto" flat="true">
              <v-container>
                <v-row justify="space-between">
                  <v-col cols="auto">
                    <v-img
                      height="180"
                      width="234.45"
                      src="https://user-images.githubusercontent.com/54254402/88759512-e92beb00-d1a5-11ea-897f-4618e0223441.png"
                    ></v-img>
                  </v-col>

                  <v-col cols="auto" class="text-center pl-0">
                    <v-row
                      class="flex-column ma-0 fill-height"
                      justify="center"
                    >
                      <v-col class="px-0"> </v-col>
                      <v-col class="px-0"> </v-col>
                      <div class="text-h2 mb-6 text-center">이란?</div>
                    </v-row>
                  </v-col>
                </v-row>
              </v-container>
            </v-card>

            <v-card-text class="text--primary">
              <div class="text-h6">
                <span class="text-h4" style="color:#26A69A">어울림</span>은 서로
                잘 조화된다는 의미입니다.
              </div>
              <div class="text-h6">
                층간소음으로 갈등을 겪는 사람들이 저희가 만든 무드등을 통해
                <b>분쟁없이 서로 조화롭게 어울리기를 바라는 마음</b>이 담긴
                팀명입니다.
              </div>
            </v-card-text>
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
            <v-card-title>어울림이란</v-card-title>

            <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>

            <v-card-text class="text--primary">

              <div>왼쪽의 통계를 보면 소음 ․ 진동민원의 발생이 늘어나고 있음을 확인할 수 있습니다.</div>
              <div></div>
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
          <v-col cols="auto">
            <v-img
              height="350"
              width="350"
              src="https://cdn.vuetifyjs.com/images/cards/store.jpg"
            ></v-img>
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
