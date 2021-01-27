<script>
    import { Col, Container, Row, Badge } from 'sveltestrap';
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Badges</b></h4>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title">
                <h5><b>Basic</b></h5>
                <p class="text-12 mgb-0">We using badge from sveltestrap, you can see full documentation in storybooks of sveltestrap.</p>
            </div>
            <div class="card-body">
                <Col md=12 class="mgb-20">
                    <h5>Default Badges</h5>
                    <p class="text-12">You can create it with properties <code>color='[primary, secondary, success, danger, warning, info, light, dark]'</code></p>
                    <Badge>Default</Badge>
                    <Badge color='primary'>Primary</Badge>
                    <Badge color='secondary'>secodary</Badge>
                    <Badge color='success'>success</Badge>
                    <Badge color='danger'>danger</Badge>
                    <Badge color='warning'>warning</Badge>
                    <Badge color='info'>Info</Badge>
                    <Badge color='light'>Light</Badge>
                    <Badge color='dark'>Dark</Badge>
                </Col>
                <Col md=12 class="mgb-20">
                    <h5>Large Badges</h5>
                    <p class="text-12">You can create it with add class <code>lg-badge</code></p>
                    <Badge class="lg-badge">Default</Badge>
                    <Badge color='primary'  class="lg-badge">Primary</Badge>
                    <Badge color='secondary' class="lg-badge">secodary</Badge>
                    <Badge color='success' class="lg-badge">success</Badge>
                    <Badge color='danger' class="lg-badge">danger</Badge>
                    <Badge color='warning' class="lg-badge">warning</Badge>
                    <Badge color='info' class="lg-badge">Info</Badge>
                    <Badge color='light' class="lg-badge">Light</Badge>
                    <Badge color='dark' class="lg-badge">Dark</Badge>
                </Col>
                <Col md=12>
                    <h5>Very Large Badges</h5>
                    <p class="text-12">You can create it with add class <code>vlg-badge</code></p>
                    <Badge class="vlg-badge">Default</Badge>
                    <Badge color='primary'  class="vlg-badge">Primary</Badge>
                    <Badge color='secondary' class="vlg-badge">secodary</Badge>
                    <Badge color='success' class="vlg-badge">success</Badge>
                    <Badge color='danger' class="vlg-badge">danger</Badge>
                    <Badge color='warning' class="vlg-badge">warning</Badge>
                    <Badge color='info' class="vlg-badge">Info</Badge>
                    <Badge color='light' class="vlg-badge">Light</Badge>
                    <Badge color='dark' class="vlg-badge">Dark</Badge>
                </Col>
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title">
                <h5><b>More Badge</b></h5>
                <p class="text-12 mgb-0">We create it to build more badges resource for your.</p>
            </div>
            <div class="card-body">
                <Col md=12 class="mgb-20">
                    <h5>Glow Badges</h5>
                    <p class="text-12">You can create it with add class <code>badge-glow</code></p>
                    <Badge class="lg-badge badge-glow">Default</Badge>
                    <Badge color='primary' class='lg-badge badge-glow'>Primary</Badge>
                    <Badge color='secondary' class='lg-badge badge-glow'>Secodary</Badge>
                    <Badge color='success' class='lg-badge badge-glow'>Success</Badge>
                    <Badge color='danger' class='lg-badge badge-glow'>Danger</Badge>
                    <Badge color='warning' class='lg-badge badge-glow'>Warning</Badge>
                    <Badge color='info' class='lg-badge badge-glow'>Info</Badge>
                    <Badge color='light' class='lg-badge badge-glow'>Light</Badge>
                    <Badge color='dark' class='lg-badge badge-glow'>Dark</Badge>
                </Col>
                <Col md=12 class="mgb-20">
                    <h5>Light Badges</h5>
                    <p class="text-12">You can create it with add class <code>lg-[default, primary, secondary, success, danger, warning, info, light, dark]</code> and add attribute <code>mode-badge='light'</code></p>
                    <Badge class="lg-badge light-default" mode-badge='light'>Default</Badge>
                    <Badge class="lg-badge light-primary" mode-badge='light'>Primary</Badge>
                    <Badge class="lg-badge light-secondary" mode-badge='light'>Secodary</Badge>
                    <Badge class="lg-badge light-success" mode-badge='light'>Success</Badge>
                    <Badge class="lg-badge light-danger" mode-badge='light'>Danger</Badge>
                    <Badge class="lg-badge light-warning" mode-badge='light'>Warning</Badge>
                    <Badge class="lg-badge light-info" mode-badge='light'>Info</Badge>
                    <Badge class="lg-badge light-light" mode-badge='light'>Light</Badge>
                    <Badge class="lg-badge light-dark" mode-badge='light'>Dark</Badge>
                </Col>
            </div>
        </div>
    </Col>
</div>