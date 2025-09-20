<script>

  import Router from 'svelte-spa-router';
  import Home from './pages/Home.svelte';
  import Projects from './pages/Projects.svelte';
  import Contact from './pages/Contact.svelte';

  const routes = {
    '/': Home,
    '/projects': Projects,
    '/contact': Contact
  };

  import {
    Button,
    Card,
    CardBody,
    CardFooter,
    CardHeader,
    CardSubtitle,
    CardText,
    CardTitle,
    Navbar,
    Nav,
    NavItem,
    NavLink,
    NavbarBrand
  } from 'sveltestrap';

</script>

<main style="max-width: 100%;">
  <div class="navTitle">
  <Navbar color="light" light expand="md" container="md">
  <NavbarBrand href="#/" style="font-size: 5vh;">Eric Gutiérrez</NavbarBrand>
    <Nav class="ms-auto" navbar>
      <NavItem>
        <NavLink href="#/" style="font-size: 2.5vh;">Home</NavLink>
      </NavItem>
      <NavItem>
        <NavLink href="#/projects" style="font-size: 2.5vh;">Projects</NavLink>
      </NavItem>
      <NavItem>
        <NavLink href="#/contact" style="font-size: 2.5vh;">Contact</NavLink>
      </NavItem>
    </Nav>
  </Navbar>
  <Router {routes} />  
  </div>
</main>

<footer style="padding-top: 3vh; padding-bottom: 1vh;">
  <p>&copy Eric Gutiérrez. 2025.</p>
</footer>

<style>
main {
  display: flex;
  flex-direction: column;    /* stack items vertically */
  justify-content: center;   /* center vertically */
  align-items: center;       /* center horizontally */
  width: 100vw;
}
.navTitle {
    width: 80%;
}

footer {
  text-align: center;
}

</style>