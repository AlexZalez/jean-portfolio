<script setup>

const hardSkills = [
{   
    text:'Payroll processing and management',
    icon:''
},
{   
    text:'Client onboarding and integration',
    icon:''
},
{   
    text:'Report creation and analysis',
    icon:'mdi-file-chart'
},
{   
    text:'Banking and accounting coordination',
    icon:'mdi-bank'
},
{   
    text:'Payroll software proficiency',
    icon:'mdi-abacus'
},
{   
    text:'Knowledge of compliance and regulatory requirements',
    icon:'mdi-head-cog-outline'
},
{   
    text:'Proficiency in Excel',
    icon:'mdi-microsoft-excel'
},
{   
    text:'Proficiency in Power BI',
    icon:''
},
{   
    text:'Proficiency in QuickBooks',
    icon:''
},
{   
    text:'Proficiency in Ledger',
    icon:'mdi-size-l'
},
]

</script>

<template>
    <div class="bg-white px-16">
        <div class="d-flex justify-center align-center py-10">
            <v-divider class="opacity-50 border-black" style="max-width: 300px;" thickness="3" />
            <span class="px-3 text-h5" >Hard Skills</span>
            <v-divider class="opacity-50 border-black" style="max-width: 300px;" thickness="3" />
        </div>

        <div class="d-flex flex-wrap justify-center ga-3">
            <v-alert 
                v-for="skill in hardSkills" 
                style="min-width: 300px;" 
                variant="tonal"
                color="blue-accent-2"
            >
                <v-list-item>
                    <v-avatar variant="tonal" color="blue">
                        <v-icon 
                            :icon="!!skill?.icon ? skill.icon : 'mdi-cash-sync'"
                        />
                    </v-avatar>
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