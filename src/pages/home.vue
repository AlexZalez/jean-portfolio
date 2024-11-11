<script setup>
import perfil from '../assets/img/perfil.png'

import hardSkill from '../components/sections/hardSkills.vue'
import softSkill from '../components/sections/softSkills.vue'

</script>

<template>
  <div class="d-flex px-16 bg-white">

    <div>
      <v-img 
        width="400"
        :src="perfil" 
        aspect-ratio="1/1"
      />
    </div>

    <div class="flex-fill d-flex justify-center align-center">
      <div class="text-h3">
        Payroll and Accounting Supervisor
        <div class="text-h6 text-center">
          Jean Mieres
        </div>
      </div>
    </div>
  </div>

  <!-- EXPERIENCE -->
  <experience />


  <!-- HARD SKILLS -->
   <hardSkill />

  <!-- SOFT SKILLS -->
   <softSkill />
   
</template>

