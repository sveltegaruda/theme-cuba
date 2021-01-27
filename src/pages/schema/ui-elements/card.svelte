<script>
    import { Col, Container, Row } from 'sveltestrap';
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Card</b></h4>
        </div>
    </Col>
    <Row>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Basic Card</b></h5>
                    <p class="text-12">Card Subtitle</p>
                </div>
                <div class="card-body">
                    <h6><b>Card Body</b></h6>
                    <p>
                        Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown ...
                    </p>
                </div>
                <div class="card-footer border-top-card">
                    <h6><b>Card Footer</b></h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card">
                <img src="/images/basic-components/1.jpg" class="card-image" alt="...">
                <div class="card-title pdt-15 pdb-15 pdl-30 pdr-30">
                    <h5><b>Basic Card</b></h5>
                    <p class="text-12 mgb-0">Card Subtitle</p>
                </div>
                <div class="card-body  pdt-15 pdb-15 pdl-30 pdr-30">
                    <h6><b>Card Body</b></h6>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                </div>
                <div class="card-footer border-top-card pdt-15 pdb-15 pdl-30 pdr-30">
                    <a href="./">Lihat Selengkapnya</a>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pdh-30 pdv-15">
                <div class="card-title">
                    <h5><b>Basic Card</b></h5>
                    <p class="text-12 mgb-0">Card Subtitle</p>
                </div>
                <div class="card-body">
                    <img src="/images/basic-components/2.jpg" class="card-image" alt="...">
                    <p class="mgt-10">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                </div>
                <div class="card-footer border-top-card">
                   <button class="btn-app bg-blue xs-btn">Lihat selengkapnya</button>
                </div>
            </div>
        </Col>
    </Row>
</div>