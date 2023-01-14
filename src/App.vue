<script setup lang="ts">
import SearchBar from './components/SearchBar.vue';
import MapView from './components/MapView.vue';
import InfoBox from './components/InfoBox.vue';
</script>

<template>
    <div class="bg-top">
      <div>
        <h1 class="title">IP Address Tracker</h1>
        <SearchBar></SearchBar>
      </div>
      <InfoBox></InfoBox>
    </div>
    <MapView></MapView>
</template>

<style scoped>
  .bg-top{
    background: url('./assets/pattern-bg.png');
    background-repeat: no-repeat;
    background-size: cover;
    height: var(--top-height);
    display: grid;
    place-items: center;
    position: relative;
  }
  .title{
    color: white;
    margin-top: 0;
    text-align: center;
    margin-bottom: 2.5rem;
    font-style: normal;
    font-weight: var(--fw-2);
  }
</style>
