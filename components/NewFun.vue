<template>
  <div>
    <h2>{{ message }}</h2>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from "vue-property-decorator";

@Component
export default class NewFunComponent extends Vue {
@Prop({ default: 'default value' }) message!: string;

}
</script>