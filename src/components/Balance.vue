<template>
    <div class="balance-container">
      <h3>Your Balance</h3>
      <h1 id="balance">${{ total.toFixed(2) }}</h1>
    </div>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    total: {
      type: Number,
      required: true,
    }
  });
  </script>