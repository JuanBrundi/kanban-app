<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">KANBAN</a>
      <div class="collapse navbar-collapse" id="navbarText">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
          </li>
        </ul>
        <span class="navbar-text">
          <a class="nav-link" href="#" @click.prevent="logout">Logout</a>
        </span>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
    // props: ["logout"],
    methods: {
        logout(){
          localStorage.clear()
          this.$emit("logout")
        }
    }
}
</script>

<style>

</style>