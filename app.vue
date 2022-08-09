<script lang="ts" setup>
// import { ulid } from "ulid";

async function onClick() {
  const { ulid } = await import(`ulid`);
  console.log(ulid());
}
</script>

<template>
  <div>
    <button @click="onClick">button1</button>
  </div>
</template>
