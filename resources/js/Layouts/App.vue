<template>
  <div>
    <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
      <div class="container">
        <inertia-link class="navbar-brand" href="/">CRUDLI</inertia-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
          <ul class="navbar-nav me-auto mb-2 mb-md-0">
            <li class="nav-item">
              <Link class="nav-link" href="/posts/">POSTS</Link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    
    <main class="container mt-5">
      <slot />
    </main>
  </div>
</template>

<script>

	

  //import Link dari inertia
  import { Link } from '@inertiajs/inertia-vue3';
  

  export default {
		

    //register Link di component
    components: {
      Link
    },
  }
</script>

<style scoped>
    .mt-5 {
      margin-top: 100px!important;
    }
</style>