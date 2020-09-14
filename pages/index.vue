<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">nuxt-app-project</h1>
      <fun-component></fun-component>
      <NewFun message="Having extra fun" />
      <div class="links">
        <NuxtLink to="/fun">Fun Page</NuxtLink>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from "vue-property-decorator";
import FunComponent from "./fun.vue";

@Component({
  components: {
    FunComponent,
  },
  // apollo: {
  //   hello: gql`query {
  //     hello
  //   }`,
  // },
})
export default class YourComponent extends Vue {}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
