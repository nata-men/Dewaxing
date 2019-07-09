<template>
  <v-app>
    <v-content   style="background-color: #E8F5E9">
        <v-toolbar
        fixed=true
        color=#4CAF50
        dark>
        <v-toolbar-title>Онлайн модель установки по депарафинизации</v-toolbar-title>
        </v-toolbar>
        <sensors/>
        <errorSignals/>
        <work/>
    </v-content>       
  </v-app>
</template>

<script>
import sensors from './components/sensors'
import errorSignals from './components/errorSignals'
import work from './components/work'

export default {  
  components: {
    sensors, 
    errorSignals,
    work
  },
    data (){
        return {}
        
    }
}
</script>
