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

<main>
  <div class="navTitle">
  <Navbar color="light" light expand="md" container="md">
  <NavbarBrand href="/" style="font-size: 2vw;">Eric Gutiérrez</NavbarBrand>
    <Nav class="ms-auto" navbar>
      <NavItem>
        <NavLink href="#/">Home</NavLink>
      </NavItem>
      <NavItem>
        <NavLink href="#/projects">Projects</NavLink>
      </NavItem>
      <NavItem>
        <NavLink href="#/contact">Contact</NavLink>
      </NavItem>
    </Nav>
  </Navbar>
  <Router {routes} />  
  </div>
</main>


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

</style>