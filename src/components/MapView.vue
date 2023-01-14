<script lang="ts" setup>
import "leaflet/dist/leaflet.css";
import L from "leaflet";
import { onMounted } from "vue";

const mapSetup = () => {
    const map = L.map("map").setView([51.505, -0.09], 13);

    L.tileLayer("https://tile.openstreetmap.org/{z}/{x}/{y}.png", {
        maxZoom: 19,
        attribution:
            '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>',
    }).addTo(map);
};

onMounted(() => {
    mapSetup();
});
</script>

<template>
    <div class="mapContainer">
        <div id="map"></div>
    </div>
</template>

<style scoped>
.mapContainer {
    width: 100%;
    height: calc(100% - var(--top-height));
}
#map{
    height: 100%;
    width: 100%;
}
</style>
