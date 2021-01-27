<script>
    import { Col, Container, Row, Alert } from 'sveltestrap';

    let visible1 = true;
    let visible2 = true;
    let visible3 = true;
    let visible4 = true;
    let visible5 = true;
    let visible6 = true;
    let visible7 = true;
    let visible8 = true;
    let visible9 = true;
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Alerts</b></h4>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title">
                <h5><b>Basic</b></h5>
                <p class="text-12">We using badge from sveltestrap, you can see full documentation in storybooks of sveltestrap.</p>
            </div>
            <div class="card-body">
                <Row>
                    <Col md=4>
                        <Alert>
                            <h4 class="alert-heading text-capitalize">Default</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='primary'>
                            <h4 class="alert-heading text-capitalize">Primary</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='secondary'>
                            <h4 class="alert-heading text-capitalize">Secondary</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='success'>
                            <h4 class="alert-heading text-capitalize">Success</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='danger'>
                            <h4 class="alert-heading text-capitalize">Danger</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='warning'>
                            <h4 class="alert-heading text-capitalize">Warning</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='info'>
                            <h4 class="alert-heading text-capitalize">Info</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='light'>
                            <h4 class="alert-heading text-capitalize">Light</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='dark'>
                            <h4 class="alert-heading text-capitalize">Dark</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                </Row>
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title">
                <h5><b>Dismissible</b></h5>
                <p class="text-12">Basicly default by sveltestrap you can get it without fade animation, but for example we using fade to more animated.</p>
            </div>
            <div class="card-body">
                <Row>
                    <Col md=4>
                        <Alert isOpen={visible1} toggle={() => (visible1 = false)}>
                            <h4 class="alert-heading text-capitalize">Default</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='primary' isOpen={visible2} toggle={() => (visible2 = false)}>
                            <h4 class="alert-heading text-capitalize">Primary</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='secondary' isOpen={visible3} toggle={() => (visible3 = false)}>
                            <h4 class="alert-heading text-capitalize">Secondary</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='success isOpen={visible4} toggle={() => (visible4 = false)}'>
                            <h4 class="alert-heading text-capitalize">Success</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='danger' isOpen={visible5} toggle={() => (visible5 = false)}>
                            <h4 class="alert-heading text-capitalize">Danger</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='warning' isOpen={visible6} toggle={() => (visible6 = false)}>
                            <h4 class="alert-heading text-capitalize">Warning</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='info' isOpen={visible7} toggle={() => (visible7 = false)}>
                            <h4 class="alert-heading text-capitalize">Info</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='light' isOpen={visible8} toggle={() => (visible8 = false)}>
                            <h4 class="alert-heading text-capitalize">Light</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                    <Col md=4>
                        <Alert color='dark' isOpen={visible9} toggle={() => (visible9 = false)}>
                            <h4 class="alert-heading text-capitalize">Dark</h4>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href="#todo" class="alert-link">Also, alert-links are colored to match</a>.
                        </Alert>
                    </Col>
                </Row>
            </div>
        </div>
    </Col>
</div>