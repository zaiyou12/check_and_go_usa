<template>
  <header class="flex flex-col items-center w-full max-w-4xl mx-auto px-2 pb-14">
    <a class="max-w-xl" href="./">
      <img alt="Check and go logo" :src="logo" />
    </a>
    <h1 class="text-4xl pb-8">Check and Go - USA</h1>
    <p class="text-base">미국 대학교-대학원 입학후 비자 준비부터 미국에서 부딪히는 다양한 문제들까지, Check & Go에서 미리 알아보고 확인하세요.</p>
  </header>
</template>

<script setup lang="ts">
import logo from '../assets/logo.png'
</script>
