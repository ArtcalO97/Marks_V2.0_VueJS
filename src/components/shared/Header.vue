
<template>
  <header id="header">
    <div class="logo">
      <router-link to="/">Marks Management</router-link>
    </div>
    <nav>
      <ul class="nav nav-pills">
 		<router-link to="/" tag="li" active-class="active" exact><a>Home</a></router-link>
 		<router-link to="/student" tag="li" active-class="active" ><a>Students</a></router-link>
 		<router-link to="/course" tag="li" active-class="active" ><a>Courses</a></router-link>
 		<router-link to="/mark" tag="li" active-class="active" ><a>Marks</a></router-link>
	</ul>
    </nav>
  </header>
</template>

<script>
  export default {
    
  };
</script>

<style scoped >
  #header {
    height: 56px;
    display: flex;
    flex-flow: row;
    justify-content: space-between;
    align-items: center;
    background-color: #521751;
    padding: 0 20px;
  }

  .logo {
    font-weight: bold;
    color: white;
  }

  .logo a {
    text-decoration: none;
    color: white;
  }

  nav {
    height: 100%;
  }

  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    height: 100%;
    display: flex;
    flex-flow: row;
    align-items: center;
  }

  li {
    margin: 0 16px;
  }

  li a {
    text-decoration: none;
    color: white;
  }

  li a:hover,
  li a:active,
  li a.router-link-active {
    color: #fa923f;
  }

  .logout {
    background-color: transparent;
    border: none;
    font: inherit;
    color: white;
    cursor: pointer;
  }
</style>