<script>
    import { Card, CardBody, CardTitle, CardText, CardFooter, CardImg, Row, Col} from 'sveltestrap';
    import { Button} from 'sveltestrap';

    const galleryItems = [
    { id: 4, title: "Neighborhood Explorer. Visualizing Socioeconomic Data at the Neighborhod Level", date: "July 2025", img: "src/lib/neighborhood-explorer.png", topics: ['Demography'], lang: 'English', type: 'Project'},
    { id: 3, title: "Un Índex de Pobresa Multidimensional per a la Regió Metropolitana de Barcelona", date: "July 2025", img: "src/lib/ipm-rmb.png", topics: ['Poverty', 'Demography'], lang: 'Catalan', type: 'Thesis', link: '/un_index_de_pobresa_multidimensional_per_a_la_rmb.pdf' },
    { id: 2, title: "Caracterización de la Distribución Espacial de las Empresas Españolas en BME y BME Growth", date: "April 2025", img: "src/lib/bme.png", topics: ['Business', 'GIS'], lang: 'Spanish', type: 'Project', link: '/caracterizacion-distribucion-espacial-bme-bme-growth.pdf'},
    { id: 1, title: "Land Use Diversity and Socioeconomic Welfare: the Case of the Barcelona Metropolitan Region", date: "June 2024", img: "src/lib/land-use.png", topics: ['Urbanism'], lang: 'English', type: 'Project', link: '/land_use_diversity_and_socioeconomic_welfare.pdf'}
  ];
</script>

<div id="gallery">

<Row>
  {#each galleryItems as item}
    <Col sm="6" md="4" lg="3" class="mb-4">
      <Card id="galleryCard">
        <div style="height: 28vh; width: auto; text-align: center; overflow: hidden; align-items: center;">
          <CardImg top src={item.img} alt={item.title} style="height: auto; width: 100%;"/>
        </div>
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
