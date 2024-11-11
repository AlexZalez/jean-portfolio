<script setup>


const messagesOne = [
'Supervise and manage comprehensive payroll processes, ensuring accuracy and compliance with regulations.',

'Implement onboarding processes for over 30 new clients, streamlining integration into payroll systems.',

'Collaborate closely with the banking department to handle reportingand accounting matters efficiently.',

'Lead and manage a team of 10 people, providing guidance and support to ensure high performance.',

'Create and analyze payroll reports, providing valuable insights for decision-making and reduced payroll errors by 15% through implementing streamlined verification procedures.',

'Communicate effectively with internal teams and external clients to ensure seamless payroll operations.',
]

const messagesTwo = [
    {title:"Started as a Payroll Assistant, managing payroll processing for 30 companies with varying pay cycles (weekly, bi-weekly, semi-monthly, and monthly) for over 1,500 employees."},
    {title:"Maintained consistent communication with each primary contact, efficiently handling all requests via email and phone."},

    {
    title:'Advanced to Payroll Specialist, expanding responsibilities to:',
    sublist:[
            'Supervise a team of 15, ensuring seamless payroll procedures.',
            'Provide support to team members with key payroll tasks.',
            'Training new hires for smooth integration and operational efficiency.',
        ]
    }
]

</script>

<template>
    <div>
        <div class="d-flex justify-center align-center py-10">
        <v-divider style="max-width: 300px;" thickness="3" />
        <span class="px-3 text-h5" >Experience</span>
        <v-divider style="max-width: 300px;" thickness="3" />
        </div>

        <v-row>
        <v-col md="6" cols="12" class="d-flex justify-center">
            <v-card 
            title="Payroll Supervisor - ResQHR" 
            subtitle="Medellín, Colombia – May 2023 – Present"
            max-width="600"
            >
            <v-timeline align="start" density="compact">
                <v-timeline-item
                v-for="(message, idx) in messagesOne"
                :key="idx"
                dot-color="blue"
                size="x-small"
                >
                <div class="mb-4">
    
                    <div>{{ message }}</div>
                </div>
                </v-timeline-item>
            </v-timeline>
            </v-card>
        </v-col>
        
        <v-col md="6" cols="12" class="d-flex justify-center">
            <v-card 
            title="Payroll Assistant / Specialist – VensureHR" 
            subtitle="Medellín, Colombia – February 2021 – May 2023"
            max-width="600"
            >
            <v-timeline align="start" density="compact">
                <v-timeline-item
                v-for="(message, idx) in messagesTwo"
                :key="idx"
                dot-color="blue"
                size="x-small"
                >
                <div class="mb-4">
    
                    <div>{{ message.title }}</div>
                </div>
                </v-timeline-item>
            </v-timeline>
            </v-card>
        </v-col>
        </v-row>
    </div>
</template>


<style lang="scss" scoped>

</style>