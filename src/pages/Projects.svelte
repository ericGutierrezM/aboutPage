<script>
    import { Card, CardBody, CardTitle, CardText, CardFooter, CardImg, Row, Col} from 'sveltestrap';
    import { Button} from 'sveltestrap';

    const galleryItems = [
    { id: 5, title: "Neighborhood Explorer. Visualizing Socioeconomic Data at the Neighborhod Level", date: "July 2025", img: "https://picsum.photos/300/200?random=1", topics: ['Demography'], lang: 'English', type: 'Project', link: "#"},
    { id: 4, title: "Neighborhood Explorer. Visualizing Socioeconomic Data at the Neighborhod Level", date: "July 2025", img: "https://picsum.photos/300/200?random=1", topics: ['Demography'], lang: 'English', type: 'Project'},
    { id: 3, title: "Un Índex de Pobresa Multidimensional per a la Regió Metropolitana de Barcelona", date: "July 2025", img: "https://picsum.photos/300/200?random=2", topics: ['Poverty', 'Demography'], lang: 'Catalan', type: 'Thesis' },
    { id: 2, title: "Caracterización de la Distribución Espacial de las Empresas Españolas en BME y BME Growth", date: "April 2025", img: "https://picsum.photos/300/200?random=3", topics: ['Business', 'GIS'], lang: 'Spanish', type: 'Project' },
    { id: 1, title: "Land Use Diversity and Socioeconomic Welfare: the Case of the Barcelona Metropolitan Region", date: "June 2024", img: "https://picsum.photos/300/200?random=1", topics: ['Urbanism'], lang: 'English', type: 'Project'}
  ];
</script>

<div id="gallery">

<Row>
  {#each galleryItems as item}
    <Col sm="6" md="4" lg="3" class="mb-4">
      <Card id="galleryCard">
        <CardImg top src={item.img} alt={item.title} />
        <CardBody>
          <CardTitle>{item.title}</CardTitle>
          <div id="cardText">
            <CardText><i class="bi bi-clock me-2"></i>{item.date}</CardText>
            <CardText><i class="bi bi-arrow-up-right-circle me-2"></i><a href="{item.link}" style="color: brown; font-weight: bold; font-style: normal;">Open</a></CardText>
          </div>
        </CardBody>
        <CardFooter>
          <div id="badges">
            <div>
              <Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>{item.topics ? item.topics[0] : ''}</Button>
              <Button style="background-color: rgb(0, 54, 23); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>{item.topics ? item.topics[1] : ''}</Button>
            </div>
            
            <div>
              <Button style="background-color: rgb(1, 121, 51); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>{item.lang}</Button>
              <Button style="background-color: rgb(27, 180, 91); color: white; border: none;" size="sm" class="rounded-pill px-2 py-0" disabled>{item.type}</Button>
            </div>


          </div>
        </CardFooter>
      </Card>
    </Col>
  {/each}
</Row>
</div>

<style>
  #gallery {
    padding-top: 2vh;
    max-width: 100%;
  }

  #cardText {
    display: flex;
    justify-content: space-between;
    padding-top: 1vh;
  }

  #badges {
    display: flex;
    justify-content: space-between;
    padding-top: 1vh;
  }

  #galleryCard {
    width: 2%;
  }

</style>
