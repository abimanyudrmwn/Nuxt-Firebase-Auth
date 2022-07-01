<template>
  <div class="flex flex-column align-start align-self-start justify-start">
    <h1>Welcome to dashboard</h1>
    <p>You are now logged in as {{ $nuxt.$fire.auth.currentUser.displayName }} ({{ $nuxt.$fire.auth.currentUser.email }})</p> 
    <v-btn
      @click="$router.push('/auth/signout')"
      >
      Logout
    </v-btn>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
