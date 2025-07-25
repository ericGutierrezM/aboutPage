<script>
  import {
    Button,
    Card,
    CardBody,
    CardFooter,
    CardHeader,
    CardSubtitle,
    CardText,
    CardTitle,
    CardImg,
    Navbar,
    Nav,
    NavItem,
    NavLink,
    NavbarBrand,
    ListGroup,
    ListGroupItem
  } from 'sveltestrap';
</script>

<div style="padding-top: 2vh; padding-bottom: 2vh;">

<Card>
  <CardBody>
    <CardTitle>About</CardTitle>
    <CardSubtitle>MSc Data Science for Decision Making | BSc Management of Smart and Sustainable Cities</CardSubtitle>
    <CardText>About text</CardText>
  </CardBody>
</Card>

</div>

<div class = 'latest'>

<Card style="width: 49.5%;">
        <CardImg top src='src/lib/neighborhood-explorer.png'/>
        <CardBody>
          <CardTitle>Latest project</CardTitle>
          <CardText></CardText>
          <CardText></CardText>
        </CardBody>
      </Card>

<Card style="width: 49.5%;">
  <CardBody>
    <CardTitle>Currently working on ...</CardTitle>
    <CardSubtitle>MSc Data Science for Decision Making | BSc Management of Smart and Sustainable Cities</CardSubtitle>
    <CardText>About text</CardText>
    <ListGroup>
      <ListGroupItem style="display: flex; justify-content: space-between; align-items: center;"><p>Hiking Trails Mapping</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>GIS</Button></ListGroupItem>
      <ListGroupItem style="display: flex; justify-content: space-between; align-items: center;"><p>Floor Area Ratio Playground</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>Urbanism</Button></ListGroupItem>

    </ListGroup>
  </CardBody>
</Card>
</div>



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

.latest {
    display: flex;
    align-items: center;
    width: 100%;
    justify-content: space-between;
}

</style>