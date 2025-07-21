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
    NavbarBrand
  } from 'sveltestrap';
</script>

<div>

<Card>
  <CardBody>
    <CardTitle>About</CardTitle>
    <CardSubtitle>MSc Data Science for Decision Making | BA Management of Smart and Sustainable Cities</CardSubtitle>
    <CardText>About text</CardText>
  </CardBody>
</Card>

</div>

<div class = 'latest'>

<Card>
        <CardImg top src='https://picsum.photos/300/200?random=1'/>
        <CardBody>
          <CardTitle>Latest project</CardTitle>
          <CardText></CardText>
          <CardText></CardText>
        </CardBody>
      </Card>

<Card>
  <CardBody>
    <CardTitle>Currently working on ...</CardTitle>
    <CardSubtitle>MSc Data Science for Decision Making | BA Management of Smart and Sustainable Cities</CardSubtitle>
    <CardText>About text</CardText>
  </CardBody>
</Card>



</div>

  <Card>
    <CardHeader>
      <CardTitle>Card title</CardTitle>
    </CardHeader>
    <CardBody>
      <CardSubtitle>Card subtitle</CardSubtitle>
      <CardText>Some quick example text to build on the card title and make up the bulk of the card's content.</CardText>
      <Button>Button</Button>
    </CardBody>
    <CardFooter>Footer</CardFooter>
  </Card>

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
}

</style>