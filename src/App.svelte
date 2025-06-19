<script>
  import Router from 'svelte-spa-router';

  import Dashboard from './pages/Dashboard.svelte';
  import RegistreraData from './pages/RegistreraData.svelte';
  import Personal from './pages/Personal.svelte';

  const routes = {
    '/': Dashboard,
    '/RegistreraData': RegistreraData,
    '/personal': Personal
  };
</script>

<nav class="p-4 bg-gray-100 flex gap-4">
  <a href="#/">Dashboard</a>
  <a href="#/RegistreraData">Registrera data</a>
  <a href="#/personal">Personal</a>
</nav>

<main class="p-4">
  <Router {routes} />
</main>
