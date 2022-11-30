<template>
  <div class="main">
    <form class="row g-3 needs-validation" id="auth-form">
      <div class="form">
        <legend><h1><b>Log in</b></h1></legend>
        <div class="mb-3">
          <label for="email" class="form-label"><span>Email</span></label>
          <input type="email" class="form-control" id="email" autofocus required>
          <span class="valid-feedback"></span>
          <span class="invalid-feedback">Please select a valid email.</span>
        </div>
        
        <div class="mb-3">
          <label for="password" class="form-label"><span>Password</span></label>
          <input type="password" class="form-control" id="password" required>
          <span class="valid-feedback"></span>
          <span class="invalid-feedback">Please select a valid password.</span>
        </div>
        <div class="mb-3 d-grid gap-2 mx-auto">
          <button type="submit" class="btn btn-primary">Log In</button>
        </div> 
      </div>

      <hr />

      <div class="mb-3 d-grid gap-2 mx-auto">
        <button type="submit" class="btn btn-outline-secondary"><IconsGoogleAuth /> Log in with Google</button>
      </div>
    </form>

    <p>No account? <span id="signup">Sign up</span></p>
  </div>
</template>

<script>
import IconsGoogleAuth from '../components/icons/IconsGoogleAuth.vue'

export default {
  components: {
    IconsGoogleAuth
  }
}

</script>
<style scoped>

#auth-form{
    padding: 1em;
    display: flex;
    place-items: center;
    border: solid 0.5px rgba(0, 0, 0, 0.26);
    margin: 0 auto;
    font-weight: normal;
    background-color: white;
  }

  #signup{
    cursor: pointer;
    text-decoration-line: underline;
    color: var(--vt-c-blue);
  }
  #signup:hover{
    color: blue;
  }
  
  p{
    text-align: center;
  }

</style>