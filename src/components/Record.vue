<template>
 <div>
  <v-btn>Start recording</v-btn>  
 </div> 
</template>
<script lang="ts">
import Vue from "vue"
import { Component } from "vue-property-decorator"

// @ts-ignore
import PizzicatoRecorder from "pizzicato-recorder"
// @ts-ignore
import Pizzicato from "pizzicato"

@Component
export default class Record extends Vue{

  record() {
    PizzicatoRecorder(Pizzicato)
  }
}
</script>