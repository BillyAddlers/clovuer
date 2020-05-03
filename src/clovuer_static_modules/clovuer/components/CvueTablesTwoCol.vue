<template>
  <table class="table table-hover">
    <thead>
      <tr>
        <th scope="col"></th> <th scope="col"></th>
      </tr>
    </thead>
    <tbody>
      <tr class="table-active">
        <th scope="row">Active</th> <td>Column content</td>
      </tr>
    </tbody>
  </table>
</template>

<script lang="ts">
  import 'reflect-metadata'
  import Vue from "vue"
  import {Component, Prop} from "vue-property-decorator"

  @Component({
    name: "CvueTablesTwoCol"
  })
  export default class CvueTablesTwoCol extends Vue {
    /**
     *
     */
    @Prop()
    // eslint-disable-next-line @typescript-eslint/no-explicit-any
    public tables!: Array<Record<string, any>>;

    @Prop({default: "active"})
    public fClass!: string;

    @Prop({default: ""})
    public sClass!: string;
  }
</script>
