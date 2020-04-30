<!--
 * Welcome to Clovuer
 * The comments in each files will guide you through your very cool journey
 * discovering what Vue can do.
 -->
<template>
  <div id="app">
    <div id="nav">
      <!--
       * router-link tag is used to move the router-view
      -->
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <!--
     * This is where your content will be displayed.
     * Refer to `router/index.ts` for component that will be displayed
     * over a router.
    -->
    <router-view></router-view>
  </div>
</template>

<!--
 * Clovuer shipped with SCSS/SASS support via node-sass.
-->
<style lang="scss" src="./styles.scss"></style>
