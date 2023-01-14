<script lang="ts" setup>
import { ref } from 'vue';

let ip = ref('');
</script>

<template>
    <div class="search">
        <input v-model="ip" type="search" class="search-input" placeholder="Search for any IP Address or domain">
        <button class="search-btn">
            <i>&rsaquo;</i>
        </button>
    </div>
</template>

<style scoped>
.search{
    color: var(--darker-grey);
    display: flex;
    border: 0;
    border-radius: 10px;
}

.search > input{
    background: white;
    color: var(--darker-grey);
    border: 0;
    width: max(40rem, 10rem);
    height: 3rem;
    outline: none;
    font-size: 18px;
    padding-left: 1rem;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
}

.search > input::placeholder{
    color: var(--darker-grey);
}

.search > input:hover, .search > input:focus, .search > input:focus-visible{
    cursor: pointer;
}

.search-btn{
    background: var(--darker-grey);
    border: 0;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    color: white;
    font-size: 1.8rem;
    padding-inline: 1rem;
}

.search-btn:hover{
    cursor: pointer;
}

.search-btn:focus{
    background-color: var(--dark-grey);
}
</style>