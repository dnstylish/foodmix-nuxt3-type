<template>
  <div>
    <div class="opacity-0">{{ counter }}</div>
    <div @click="tangLen">Click me</div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "@vue/runtime-core";

const counter = ref(0)

function tangLen(): void {
  counter.value++
}

</script>

<script lang="ts">
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "HomePage"
})
</script>
