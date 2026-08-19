<template>
  <div class="container narrow">
    <h1>Create an account</h1>

    <form class="card">
      <div class="field">
        <label for="name">Name</label>
        <input id="name" required autocomplete="name" />
      </div>

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
          minlength="8"
          autocomplete="new-password"
        />
        <small class="muted">At least 8 characters.</small>
      </div>


      <button class="primary" type="submit" disabled>
       Sign up
      </button>
    </form>

    <p class="muted">
      Already have an account? <RouterLink :to="{ name: 'login' }">Log in</RouterLink>
    </p>
  </div>
</template>

<style scoped>
.narrow {
  max-width: 420px;
}
</style>
