<template>
  <table class="table table-hover">
    <thead></thead>
  </table>
</template>

<script lang="ts">
  import 'reflect-metadata'
  import Vue from "vue"
  import {Component, Prop} from "vue-property-decorator"
  import {TwoCol} from "../clovuer";

  @Component({
    name: "CvueTables"
  })
  export default class CvueTablesTwoCol extends Vue {
    @Prop
    tables: Array<TwoCol>;

    @Prop({default: "active"})
    fClass: string;

    @Prop({default: ""})
    sClass: string;

    get fClass() {
      return `table-${this.fClass}`
    }
    get sClass() {
      return `table-${this.sClass}`
    }
  }
</script>
