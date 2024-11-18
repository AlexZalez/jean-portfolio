<script setup>

</script>

<template>
    <v-app-bar
        color="primary"
        prominent
    >

        <div class="w-100 d-flex justify-center align-center ga-16">
            
            <mainLogo size="54" />

            <div
                v-if="$vuetify.display.mdAndUp"
                class="d-flex ga-0"
            >
                <v-tab v-for="nav in ['Experience', 'Hard Skills', 'Soft Skills', 'Languages', 'Contact']" >
                    {{ nav }}
                </v-tab>
            </div>

            <div>
                <v-btn icon>
                    <v-icon size="36" icon="mdi-linkedin"  />

                </v-btn>
                    <!-- class="pe-3" -->
                <v-btn 
                    v-if="$vuetify.display.smAndDown"
                    icon="mdi-dots-vertical" 
                    variant="text"
                />
            </div>

        </div>    


        


        
    </v-app-bar>
</template>


<style lang="scss" scoped>

</style>