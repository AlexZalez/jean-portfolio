<script setup>
import perfil from '../assets/img/perfil.png'
import fullperfil from '../assets/img/fullperfil.jpeg'

import hardSkill from '../components/sections/hardSkills.vue'
import softSkill from '../components/sections/softSkills.vue'

</script>

<template>
  <div class="d-flex py-16 ga-10 bg-white justify-center">

    <div class=" d-flex justify-center align-center">
      <div class="text-end">
        <div class="mb-8">
          Payroll and Accounting Manager
        </div>
        <div class="text-h1 text-blue font-weight-bold ">
          <div>JEAN </div>
          <div>MIERES</div>
        </div>
        <div class="mt-10">
          <VBtn 
            color="blue"
            append-icon="mdi-play"
            text="CONTACT"
          />
        </div>
      </div>
    </div>
    <div>
      <v-img 
        width="500"
        max-height="500"
        cover
        :src="fullperfil" 
        aspect-ratio="1/1"
      />
    </div>

  </div>

  <!-- EXPERIENCE -->
  <experience />


  <!-- HARD SKILLS -->
   <hardSkill />

  <!-- SOFT SKILLS -->
   <softSkill />
   
</template>

