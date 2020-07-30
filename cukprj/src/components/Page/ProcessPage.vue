<template>
  <v-container>
    <v-card max-width="900" class="mx-auto" flat>
      <v-card-title class="text-h3 mb-6 text-center"
        >제품 동작 원리</v-card-title
      >
      <v-container>
        <v-row justify="space-between">
          <v-col cols="auto">
            <v-img
              src="https://user-images.githubusercontent.com/52627952/88545546-18cbdd80-d056-11ea-9b45-5a2d2a9bebcb.gif"
            ></v-img>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-card max-width="900" class="mx-auto" flat>
      <v-container>
        <v-row justify="space-between">
          <v-col>
            <v-img
              width="250px"
              src="https://user-images.githubusercontent.com/52627952/88758179-c9df8e80-d1a2-11ea-9ba3-e90a01c6de1d.png"
            ></v-img>
            일렉트릭 마이크로폰 앰프 모듈 / CJMCU MAX9812L<br />
            층간소음의 소음을 감지하는 역할을 하는 부품
          </v-col>
          <v-col>
            <v-img
              width="250px"
              src="https://user-images.githubusercontent.com/52627952/88758169-c815cb00-d1a2-11ea-8516-b65198aa9fa9.jpg"
            ></v-img>
            진동, 충격 센서모듈 / SW-420<br />
            층간소음의 진동을 감지하는 역할을 하는 부품
          </v-col>
        </v-row>
        <v-row justify="space-between">
          <v-col>
            <v-img
              width="250px"
              src="https://user-images.githubusercontent.com/52627952/88758175-c946f800-d1a2-11ea-89af-12617a0900b8.png"
            ></v-img>
            무선통신 모듈 / 2.4G Wireless nRF24L01P RFM04<br />
            수신기와 송신기 사이 통신을 가능하게 해주는 부품
          </v-col>
          <v-col>
            <v-img
              width="250px"
              src="https://user-images.githubusercontent.com/52627952/88758176-c9df8e80-d1a2-11ea-879c-7a918abc6309.png"
            ></v-img>
            nRF24L01 모듈용 ATMega48 개발보드<br />
            무선통신 모듈과 연결하여 무선통신을 가능하게 해주는 부품
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-card max-width="900" class="mx-auto" flat>
      <v-container>
        <v-row justify="space-between">
          <v-col cols="auto">
            <v-card-title class="text-h4">송신기</v-card-title>
            <v-img
              width="400px"
              src="https://user-images.githubusercontent.com/52627952/88759264-5d19c380-d1a5-11ea-81e3-8828badb2c3d.jpg"
            ></v-img>
          </v-col>
          <v-col cols="auto">
            <v-card-title class="text-h4">수신기</v-card-title>
            <v-img
              width="400px"
              src="https://user-images.githubusercontent.com/52627952/88759267-5e4af080-d1a5-11ea-9e58-009b8e45e1ba.png"
            ></v-img>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <br /><br />
    <h6 class="text-center">
      아이콘 제작자
      <a
        style="color: black; text-decoration: none;"
        href="https://www.flaticon.com/kr/authors/freepik"
        title="Freepik"
        >Freepik</a
      >
      | 아이콘 제작자
      <a
        style="color: black; text-decoration: none;"
        href="https://www.flaticon.com/kr/authors/flat-icons"
        title="Flat Icons"
        >Flat Icons</a
      >
      | 아이콘 제작자
      <a
        style="color: black; text-decoration: none;"
        href="https://www.flaticon.com/kr/authors/good-ware"
        title="Good Ware"
        >Good Ware</a
      >
      | from
      <a
        style="color: black; text-decoration: none;"
        href="https://www.flaticon.com/kr/"
        title="Flaticon"
      >
        www.flaticon.com</a
      >
      | 부품 이미지 출처
      <a
        style="color: black; text-decoration: none;"
        href="http://mechasolution.com/"
        title="mechasolution"
        >www.mechasolution.com</a
      >
    </h6>
  </v-container>
</template>

<script>
export default {
  name: "ProductPage",

  data: () => ({}),
};
</script>
