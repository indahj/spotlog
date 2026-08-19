<script setup lang="ts">

</script>

<template>
  <div class="container narrow">
    <h1>Log in</h1>

    <form class="card" >
      <div class="field">
        <label for="email">Email</label>
        <input id="email" type="email" required autocomplete="email" />
      </div>

      <div class="field">
        <label for="password">Password</label>
        <input
          id="password"
          type="password"
          required
          autocomplete="current-password"
        />
      </div>

      <button class="primary" type="submit" disabled>
        Log in
      </button>
    </form>

    <p class="muted">
      No account yet? <RouterLink :to="{ name: 'register' }">Sign up</RouterLink>
    </p>
  </div>
</template>

<style scoped>
.narrow {
  max-width: 420px;
}
</style>
