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
    <div class="pb-16" >
        <div class="d-flex justify-center align-center py-10">
            <v-divider style="max-width: 300px;" thickness="3" />
            <span class="px-3 text-h5 font-weight-bold" >Experience</span>
            <v-divider style="max-width: 300px;" thickness="3" />
        </div>
        
        <v-expansion-panels variant="accordion" class="mx-auto" style="max-width: 1000px;" >
            <v-expansion-panel tile >
                <v-expansion-panel-title>
                    <v-row class="d-flex align-center ga-6" >
                        <v-col cols="3" class="text-grey">
                            May 2023 – <span class="text-white">Present</span>
                        </v-col>
                        <v-col cols="auto">
                            <div class="font-weight-bold text-h6" >Payroll Supervisor - ResQHR</div>
                            <div>Medellín, Colombia</div>
                        </v-col>
                    </v-row>
                </v-expansion-panel-title>
                <v-expansion-panel-text class="overflow-auto" style="max-height: 300px;">
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
                </v-expansion-panel-text>
            </v-expansion-panel>

            <v-expansion-panel tile >
                <v-expansion-panel-title>
                    <v-row class="d-flex align-center ga-6" >
                        <v-col cols="3" class="text-grey">
                            February 2021 – May 2023
                        </v-col>
                        <v-col cols="auto" >
                            <div class="font-weight-bold text-h6" >Payroll Assistant / Specialist – VensureHR</div>
                            <div>Medellín, Colombia</div>
                        </v-col>
                    </v-row>
                </v-expansion-panel-title>
                <v-expansion-panel-text class="overflow-auto" style="max-height: 300px;">
                    <v-timeline align="start" density="compact">
                        <v-timeline-item
                            v-for="(message, idx) in messagesTwo"
                            :key="idx"
                            dot-color="blue"
                            size="x-small"
                        >
                            <div>
                                <div>{{ message.title }}</div>
                                <v-timeline align="start" class="ga-3" v-if="!!message?.sublist">
                                    <v-timeline-item
                                        v-for="(msg, index) in message.sublist"
                                        :key="index"
                                        dot-color="blue"
                                        size="x-small"
                                    >
                                        {{ msg }}
                                    </v-timeline-item>
                                </v-timeline>
                            </div>
                        </v-timeline-item>
                    </v-timeline>
                </v-expansion-panel-text>
            </v-expansion-panel>

        </v-expansion-panels>

        
    </div>
</template>