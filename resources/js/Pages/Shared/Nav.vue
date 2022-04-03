<template>
  <nav>
    <ul
      class="d-flex flex-row justify-content-around p-5 bg-warning text-decoration-none text-dark list-none"
    >
      <li class="fw-600 fw-bold display-6 text-secondary">
        EMP {{ $page.props.auth.user.username }}
      </li>
      <li>
        <NavLink href="/" :active="$page.component === 'Home'">Home</NavLink>
      </li>
      <li>
        <NavLink href="/users" :active="$page.component === 'User'">Users</NavLink>
      </li>
      <li>
        <Link
          href="/settings"
          :class="{ 'fw-bold text-white': $page.component === 'Settings' }"
          >Settings</Link
        >
      </li>
      <li><Link href="/logout" meth od="post" as="button">Logout</Link></li>
    </ul>
  </nav>
</template>

<script>
import { Link } from "@inertiajs/inertia-vue3";
import NavLink from "./NavLink.vue";
export default {
  components: { Link, NavLink },
};
</script>

<style scoped>
nav ul li {
  list-style: none;
}

nav ul li:hover {
  color: rgb(158, 158, 158);
}

li Link {
  text-decoration: none;
  color: blanchedalmond;
}
</style>
