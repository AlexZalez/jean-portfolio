<script setup>

defineProps({
    size:{
        type: Number,
        default: 60,
    }
})

</script>

<template>
    <div class="d-flex align-center ga-2">
        <v-avatar :size rounded color="white">
            <div class="text-blue font-weight-bold text-h4">
                JM
            </div>
        </v-avatar>
        <div style="letter-spacing: 0.1em;">
            <div > JEAN </div>
            <div> MIERES</div>
        </div>
    </div>
</template>


<style lang="scss" scoped>

</style>