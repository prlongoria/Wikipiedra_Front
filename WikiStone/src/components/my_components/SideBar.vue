<!-- Debo meterle funcionalidad y css correcto para que con media query cambie a la parte superior, de
momento, la he muteado de la vista HomeView. Aquí irá toda la info extra como limpiar piedras y otras
curiosidades del libro -->

<script>
export default {};
</script>
<template>
  <div id="sidebar">
    <h1>Home Page</h1>
    <nav>
      <RouterLink to="/create">CreateView</RouterLink>
      <br />
      <RouterLink to="/detail">DetailView</RouterLink>
      <br />
      <RouterLink to="/update">UpdateView</RouterLink>
    </nav>
  </div>
</template>

<style scoped>
#sidebar {
  display: flex;
  flex-direction: column;
  width: 12vw;
  font-size: 2vw;
  background-color: var(--primary-color);
  margin: 1vw;
  color: whitesmoke;
}

@media all and (max-width: 840px) {
  #sidebar {
    display: block;
    flex-direction: column;
    width: 12vw;
    font-size: 2vw;
    background-color: var(--primary-color);
    margin: 1vw;
    color: whitesmoke;
  }
}

h1 {
  font-size: 3vw;
}

</style>
