<template>
  <div id="app">
      <h1> Let's go home</h1>
      <hr>
        <router-link to="/users/10">Users</router-link>
      <hr>
      <router-view></router-view>
  </div>
</template>

<script>
export default {
  data () {
    return {
        
    }
  }
}
</script>
