<script setup>

const softSkills = [
    {
        text:'Leadership and team management',
        icon:''
    },
    {
        text:'Effective communication',
        icon:''
    },
    {
        text:'Problem-solving',
        icon:''
    },
    {
        text:'Attention to detail',
        icon:''
    },
    {
        text:'Time management',
        icon:''
    },
    {
        text:'Adaptability',
        icon:''
    },
    {
        text:'Client relationship management',
        icon:''
    },
    {
        text:'Empathy',
        icon:''
    },
    {
        text:'Mentorship',
        icon:''
    },
    {
        text:'Decision-making',
        icon:''
    },
    {
        text:'Active listening',
        icon:''
    },
    {
        text:'Resilience',
        icon:''
    },
]

</script>

<template>
    <div class="bg-white px-16">
        <div class="d-flex justify-center align-center py-10">
            <v-divider class="opacity-50 border-black" style="max-width: 300px;" thickness="3" />
            <span class="px-3 text-h5" >Soft Skills</span>
            <v-divider class="opacity-50 border-black" style="max-width: 300px;" thickness="3" />
        </div>

        <div class="d-flex flex-wrap justify-center ga-3">
            <v-alert 
                v-for="skill in softSkills" 
                style="min-width: 300px;" 
                variant="tonal"
                color="blue-accent-2"
            >
                <v-list-item>
                    <!-- <v-avatar variant="tonal" color="blue">
                        <v-icon 
                            :icon="!!skill?.icon ? skill.icon : 'mdi-cash-sync'"
                        />
                    </v-avatar> -->
                    <p>
                        {{ skill.text }}
                    </p>
                </v-list-item>
            </v-alert>
        </div>
    </div>
</template>


<style lang="scss" scoped>

</style>