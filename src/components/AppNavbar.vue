<script setup>

</script>

<template>
    <v-app-bar
        color="primary"
        prominent
        density="compact"
    >

        <v-toolbar-title>
            JM
        </v-toolbar-title>

        <v-spacer></v-spacer>

        <v-tabs
            v-if="$vuetify.display.mdAndUp"
            align-tabs="center"
            class="d-flex ga-2 me-16"
        >
            <v-tab 
                v-for="nav in ['Experience', 'Hard Skills', 'Soft Skills', 'Languages', 'Contact']" 
            >
                {{ nav }}
            </v-tab>
        </v-tabs>


        <v-btn 
            icon="mdi-linkedin" 
            variant="text"
            class="pe-3"
        />
        <v-btn 
            v-if="$vuetify.display.smAndDown"
            icon="mdi-dots-vertical" 
            variant="text"
        />
    </v-app-bar>
</template>


<style lang="scss" scoped>

</style>