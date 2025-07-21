<script>
    import { Card, CardBody, CardTitle, CardText, CardFooter, CardImg, Row, Col, Badge } from 'sveltestrap';

    const galleryItems = [
    { id: 1, title: "Card 1", date: "This is card 1", img: "https://picsum.photos/300/200?random=1", badges: []},
    { id: 2, title: "Card 2", date: "This is card 2", img: "https://picsum.photos/300/200?random=2" },
    { id: 3, title: "Card 3", date: "This is card 3", img: "https://picsum.photos/300/200?random=3" },
    { id: 4, title: "Card 4", date: "This is card 4", img: "https://picsum.photos/300/200?random=4" }
  ];
</script>

<div>

<Row>
  {#each galleryItems as item}
    <Col sm="6" md="4" lg="3" class="mb-4">
      <Card>
        <CardImg top src={item.img} alt={item.title} />
        <CardBody>
          <CardTitle>{item.title}</CardTitle>
          <CardText>{item.date}</CardText>
          <CardText>{item.badges}</CardText>
        </CardBody>
        <CardFooter>badges</CardFooter>
      </Card>
    </Col>
  {/each}
</Row>
</div>