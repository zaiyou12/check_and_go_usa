<script setup lang="ts">
import MainHeader from "./components/MainHeader.vue";
import CheckList from "./components/CheckList.vue";

const title = "입학 전";
const body = [
  "유학 결심",
  "유학목표 설정",
  "학교 정보 수집 - 학교 홈페이지의 국제 학생 지원 페이지를 통해 알아보기",
  "학교 정보 수집 - 학교 국제의 국제 학생 지원 부서에 정보 요청하기",
  "학교 정보 수집 - 구글에서 검색하기",
  "학교 지원 및 지원서 제출",
];

const headers = ["입학 전", "입학 후", "도미 후"];
const checklists = [
  [
    "유학 결심",
    "유학목표 설정",
    "학교 정보 수집 - 학교 홈페이지의 국제 학생 지원 페이지를 통해 알아보기",
    "학교 정보 수집 - 학교 국제의 국제 학생 지원 부서에 정보 요청하기",
    "학교 정보 수집 - 구글에서 검색하기",
    "학교 지원 및 지원서 제출",
  ],
  [
    "여권발급",
    "여권발급",
    "I-20 받기",
    "I-901 SEVIS 수수료 내기",
    "영사관에 F1 비자 인터뷰 예약하기",
    "수업 등록하기",
    "주거 형태 결정하기",
    "비행기 예약하기",
  ],
  [
    "핸드폰 개통하기",
    "은행 계좌만들기",
    "숙소 구하기",
    "인터넷 개통하기",
    "학교 방문하여 ID카드 발급받기",
    "주변 생활 정보 익히기",
    "가구 등 생필품 구입"
  ]
];
</script>

<template>
  <MainHeader />
  <section class="mx-auto py-16 w-11/12 max-w-screen-lg">
    <CheckList
      v-for="(header, index) in headers"
      :key="index"
      :title="header"
      :body="checklists[index]"
    />
  </section>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: rgba(167, 243, 208, 0.4);
}
.max-w-screen-lg {
  max-width: 1012px;
}
</style>
