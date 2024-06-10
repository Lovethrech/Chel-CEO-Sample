<script setup>
import LogoCtn from "@/components/LogoCtn.vue";
import NavContent from '@/components/NavContent.vue'
</script>

<style scoped>
.nav-main-container{
    width:100%;
    height:7vh;
    background-color: rgba(43, 66, 80, 0.479);
}
.logo{
    width:100%;
    height:60%;
    display:flex;
    place-items:center;
    justify-content: center;
}
</style>

<template>
    <div class="nav-main-container">
        <div class="logo">
            <LogoCtn/>
        </div>
        <NavContent/>
    </div>
</template>