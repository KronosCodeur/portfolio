<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>
<style>
* {
  font-family: "Helvetica Neue", sans-serif;
}
body{
  background: #0A0E11;
}
</style>
<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
}
</script>
