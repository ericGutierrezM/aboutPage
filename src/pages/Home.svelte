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

<div style="width: 100%; display: flex; justify-content: space-between;">
<div style="padding-top: 2vh; padding-bottom: 2vh; width: 69.5%;">
<Card>
  <CardBody>
    <img src="/photo.png" style="width: 10vw; float: left; border-radius: 50%; margin-right: 2%; padding-top: 1vh; pointer-events: none;">
    <CardTitle style="font-size: 2.7vh;">About</CardTitle>
    <CardSubtitle style="padding-top: 2vh; font-size: 2.3vh;">MSc Candidate in Data Science for Decision Making @ Barcelona School of Economics</CardSubtitle>
    <CardText style="padding-top: 1.7vh; font-size: 2.2vh;"><p>I'm a <i>Data Science for Decision Making</i> student and a 
      <i>Management of Smart and Sustainable Cities</i> graduate interested in how to leverage data to enhance decision-making processes 
      in public policy and urban affairs.</p>
    <p>During my undergraduate studies, I had the opportunity to explore and
gain knowledge in many disciplines in social science, such as mobility and
public transportation, public policy, and urban planning, among others. 
Consequently, I have been introduced to the diverse (and pressing)
challenges cities, economies, and societies worldwide face.
Additionally, I have also acquired a strong foundation in technical skills, which I believe constitute excellent tools
for deepening our understanding of these challenges, with the ultimate goal of developing
effective, transparent, and creative solutions in the form of public policies.</p>
<p>At the Barcelona School of Economics, I aim to take my data science and analytics skill set to a
whole new level, unlocking new techniques and methods that will surely
prove vital and immensely enriching for my professional career. Ultimately, my goal is to build a better world
through the valuable insights data science and analytics provides.</p>
<p>When I'm not studying, chances are I'm working on some data visualization
project on virtually anything people- or place-related, or
researching on business- and economy-related topics, and particularly, in
the fields of innovation and entrepreneurship. I also love reading (I'm currently deep into John Steinbeck), listening to music, and playing the guitar.</p>
    </CardText>
  </CardBody>
</Card>

<Card style="margin-top: 2vh;">
  <CardBody>
    <CardTitle style="font-size: 2.7vh;">Latest Reads & Inspirations</CardTitle>
    <CardText style="padding-top: 1.2vh; font-size: 2.2vh;">The latest articles, books, pages (and everything in between) that I have been reading or thinking about lately. </CardText>
    <ListGroup>
      <ListGroupItem style="justify-content: space-between; align-items: center;"><p style="font-size: 2.3vh;">Políticas Públicas: Entre la deliberación y el ejercicio de la autoridad. <i>Quim Burgué Torruella</i> (2014)</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none; margin-left: 1vw;" size="sm" class="rounded-pill px-2 py-0" disabled>Article | Public Policy</Button></ListGroupItem>
      <ListGroupItem style="justify-content: space-between; align-items: center;"><p style="font-size: 2.3vh;">Hello World: How to Be Human in the Age of the Machine. <i>Hannah Fry</i> (2018)</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none; margin-left: 1vw;" size="sm" class="rounded-pill px-2 py-0" disabled>Book | Data</Button></ListGroupItem>
      <ListGroupItem style="justify-content: space-between; align-items: center;"><p style="font-size: 2.3vh;">The Rise of the Global Startup City. The New Map of Entrepreneurship and Venture Capital. <i>Richard Florida & Ian Hathaway</i> (2018)</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none; margin-left: 1vw;" size="sm" class="rounded-pill px-2 py-0" disabled>Article | Business</Button></ListGroupItem>
      <ListGroupItem style="justify-content: space-between; align-items: center;"><p style="font-size: 2.3vh;">Uprooted: Recovering the Legacy of the Places We've Left Behind. <i>Grace Olmstead</i> (2021)</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none; margin-left: 1vw;" size="sm" class="rounded-pill px-2 py-0" disabled>Book | Sociology, Community</Button></ListGroupItem>
    </ListGroup>
  </CardBody>
</Card>

</div>

<div class = 'latest'>

<Card style="width: 100%;">
  <div class="image-wrapper">
    <CardImg top src='/neighborhood-explorer.png' style="width: 100%; height: auto;"/>
    <div class="latest-label">LATEST</div>
  </div>

  <CardBody>
    <CardTitle style="font-size: 2.3vh;">Neighborhood Explorer. Visualizing Socioeconomic Data at the Neighborhod Level</CardTitle>
    <div id="cardText">
      <CardText style="font-size: 2.2vh;"><i class="bi bi-clock me-2"></i>July 2025</CardText>
      <CardText style="font-size: 2.2vh;"><i class="bi bi-arrow-up-right-circle me-2"></i><a href="#/projects" style="color: brown; font-weight: bold; font-style: normal;">Go to Projects</a></CardText>
    </div>
  </CardBody>
</Card>

<Card style="width: 100%; margin-top: 2vh;">
  <CardBody>
    <CardTitle style="font-size: 2.7vh;">Currently working on ...</CardTitle>
    <CardSubtitle></CardSubtitle>
    <CardText></CardText>
    <ListGroup>
      <ListGroupItem style="display: flex; justify-content: space-between; align-items: center; font-size: 2.2vh;"><p>Hiking Trails Mapping</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>GIS</Button></ListGroupItem>
      <ListGroupItem style="display: flex; justify-content: space-between; align-items: center; font-size: 2.2vh;"><p>Floor Area Ratio Playground</p><Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>Urbanism</Button></ListGroupItem>

    </ListGroup>
  </CardBody>
</Card>
</div>
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
    align-items: center;
    width: 29.5%;
    padding-top: 2vh; 
    padding-bottom: 2vh;
}

#cardText {
  display: flex;
  justify-content: space-between;
  padding-top: 1vh;
}

.image-wrapper {
  position: relative;
  display: inline-block;
  width: 100%;
}

.latest-label {
  position: absolute;
  top: 2%;       /* distance from top */
  left: 1.5%;      /* distance from left */
  background: rgba(0, 0, 0, 0.5); /* semi-transparent background */
  color: white;
  padding: 4px 8px;
  border-radius: 6px;
  font-size: 2.5vh;
  font-weight: bold;
}

</style>