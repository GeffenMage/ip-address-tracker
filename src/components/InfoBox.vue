<script setup lang="ts"></script>

<template>
    <div class="info-box">
        <div class="info-list">
            <section class="info-list-item">
                <h1>IP Address</h1>
                <p>192.168.1.1</p>
            </section>
            <section class="info-list-item">
                <h1>Location</h1>
                <p>Rio de Janeiro</p>
            </section>
            <section class="info-list-item">
                <h1>Timezone</h1>
                <p>GMT-3</p>
            </section>
            <section class="info-list-item">
                <h1>ISP</h1>
                <p>Vivo</p>
            </section>
        </div>
    </div>
</template>

<style scoped>
.info-box{
    position: absolute;
    background: white;
    border-radius: 10px;
    padding: 2rem;
    top: 19rem;
    z-index: 9999;
}

.info-list{
    display: flex;
    gap: 1rem;
}

.info-list-item{
    color: var(--darker-grey);
    border-right: 1px solid var(--dark-grey);
    padding: 1rem;
}
</style>