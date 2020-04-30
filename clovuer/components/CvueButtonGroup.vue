<template>
  <div class="btn-group" role="group" aria-label="Button group with nested dropdown">
    <slot></slot>
  </div>
</template>

<script lang="ts">
  import 'reflect-metadata'
  import Vue from "vue"
  import {Component} from "vue-property-decorator"

  @Component({
    name: "CvueButtonGroup"
  })
  export default class CvueButtonGroup extends Vue {}
</script>
