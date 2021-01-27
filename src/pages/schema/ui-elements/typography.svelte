<script>
    import { Col, Container, Row } from 'sveltestrap';
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Typography</b></h4>
        </div>
    </Col>
    <Row>
        <Col md=6>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Headings</b></h5>
                    <p class="text-13 mgb-0">
                        All HTML headings, <span class="tcolor-blue">h1</span> through <span class="tcolor-blue">h6</span>, are available.
                    </p>
                </div>
                <div class="card-body">
                    <h1>This is Heading</h1>
                    <h2>This is Heading</h2>
                    <h3>This is Heading</h3>
                    <h4>This is Heading</h4>
                    <h5>This is Heading</h5>
                    <h6>This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=6>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Text Color</b></h5>
                    <p class="text-13 mgb-0">
                        You can add color for your text with class tcolor- *. You can access in text.app.css
                    </p>
                    <code class="text-12">.tcolor-black, .tcolor-blue, .tcolor-teal, .tcolor-red, .tcolor-red-light, .tcolor-orange, .tcolor-green, etc..</code>
                </div>
                <div class="card-body">
                    <h1 class="tcolor-blue">This is Heading</h1>
                    <h2 class="tcolor-teal">This is Heading</h2>
                    <h3 class="tcolor-red">This is Heading</h3>
                    <h4 class="tcolor-orange">This is Heading</h4>
                    <h5 class="tcolor-green">This is Heading</h5>
                    <h6 class="tcolor-black">This is Heading</h6>
                </div>
            </div>
        </Col>
    </Row>
    <Row>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Very Thin (100)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-100">This is Heading</h1>
                    <h2 class="text-w-100">This is Heading</h2>
                    <h3 class="text-w-100">This is Heading</h3>
                    <h4 class="text-w-100">This is Heading</h4>
                    <h5 class="text-w-100">This is Heading</h5>
                    <h6 class="text-w-100">This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Thin (300)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-300">This is Heading</h1>
                    <h2 class="text-w-300">This is Heading</h2>
                    <h3 class="text-w-300">This is Heading</h3>
                    <h4 class="text-w-300">This is Heading</h4>
                    <h5 class="text-w-300">This is Heading</h5>
                    <h6 class="text-w-300">This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Normal (400)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-400">This is Heading</h1>
                    <h2 class="text-w-400">This is Heading</h2>
                    <h3 class="text-w-400">This is Heading</h3>
                    <h4 class="text-w-400">This is Heading</h4>
                    <h5 class="text-w-400">This is Heading</h5>
                    <h6 class="text-w-400">This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Light Bold (600)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-600">This is Heading</h1>
                    <h2 class="text-w-600">This is Heading</h2>
                    <h3 class="text-w-600">This is Heading</h3>
                    <h4 class="text-w-600">This is Heading</h4>
                    <h5 class="text-w-600">This is Heading</h5>
                    <h6 class="text-w-600">This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Bold (700)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-700">This is Heading</h1>
                    <h2 class="text-w-700">This is Heading</h2>
                    <h3 class="text-w-700">This is Heading</h3>
                    <h4 class="text-w-700">This is Heading</h4>
                    <h5 class="text-w-700">This is Heading</h5>
                    <h6 class="text-w-700">This is Heading</h6>
                </div>
            </div>
        </Col>
        <Col md=4>
            <div class="card pda-30">
                <div class="card-title">
                    <h5><b>Very Bold (900)</b></h5>
                </div>
                <div class="card-body">
                    <h1 class="text-w-900">This is Heading</h1>
                    <h2 class="text-w-900">This is Heading</h2>
                    <h3 class="text-w-900">This is Heading</h3>
                    <h4 class="text-w-900">This is Heading</h4>
                    <h5 class="text-w-900">This is Heading</h5>
                    <h6 class="text-w-900">This is Heading</h6>
                </div>
            </div>
        </Col>
    </Row>
</div>