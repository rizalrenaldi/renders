<template>
  <div>
    <h2>SWR: 1 &mdash; testing with data fetch</h2>
    <p>"Generated on-demand, revalidates in background", but I have no idea what it mean</p>
    <div>
      <pre>{{ data }}</pre>
    </div>
  </div>
</template>

<script setup>
const {data} = await useFetch('https://tapi-vercel.vercel.app/test')
</script>