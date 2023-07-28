<template>
  <div>
    <h2>ISR: true &mdash; testing with data fetch</h2>
    <p>Supposed to be rendered on client-side</p>
    <div>
      <pre>{{ data }}</pre>
    </div>
  </div>
</template>

<script setup>
const {data} = await useFetch('https://tapi-vercel.vercel.app/test')
</script>