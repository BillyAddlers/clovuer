<!--
 * Welcome to Clovuer
 * The comments in each files will guide you through your very cool journey
 * discovering what Vue can do.
 -->
<template>
  <div class="home">
    <img alt="Vue logo" style="height: 200px; width: 200px" src="../assets/logo.png">
    <img alt="Vue logo" style="height: 150px; width: 150px" src="../assets/heart.png">
    <img alt="Vue logo" style="height: 200px; width: 200px" src="../assets/typescript-logo.png">
    <!--
     * Vue Components can be called as easy as using HTML's custom tags
     * Some Component also have property called Prop, and can be defined
     * via HTML attribute tag.
    -->
    <HelloWorld msg="Welcome to Your Clovuer App"/>
  </div>
</template>

<script lang="ts">
  /**
   * You can use `@/` as an equivalent for `./src`
   */
  import HelloWorld from '@/components/HelloWorld.vue'
  import Vue from "vue"
  import {Component} from "vue-property-decorator"
  /**
   * @Component decorator is used to declare a Vue Component
   * and including Component into the Vue instance
   */
  @Component({
    name: "Home",
    components: {
      HelloWorld
    }
  })
  export default class Home extends Vue {}
</script>
