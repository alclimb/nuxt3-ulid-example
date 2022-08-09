<script lang="ts" setup>
// MEMO: Error with static import
// import { ulid } from "ulid";

async function onClick() {
  // Avoid errors with dynamic imports
  const { ulid } = await import(`ulid`);

  // Run ulid
  console.log(ulid());
}
</script>

<template>
  <div>
    <button @click="onClick">button1</button>
  </div>
</template>
