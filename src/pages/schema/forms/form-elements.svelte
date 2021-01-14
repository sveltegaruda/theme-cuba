<script>
    import {
        Col,
        FormGroup,
        Input,
        CustomInput,
        Row
    } from 'sveltestrap';
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Form Elements</b></h4>
        </div>
    </Col>
    <Col md="12">
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Basic Components</b></h5>
                <p class="text-12">
                    You can add this component to your apps, to build your form more marvelous.
                </p>
            </div>
            <div class="card-body">
                <Row>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Plaintext</label>
                            <Input plaintext name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Text</label>
                            <Input type="text" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Email</label>
                            <Input type="email" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Password</label>
                            <Input type="password" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Search</label>
                            <Input type="search" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">URL</label>
                            <Input type="url" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Number</label>
                            <Input type="number" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Tel</label>
                            <Input type="tel" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Range</label>
                            <Input type="range" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Date</label>
                            <Input type="date" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Month</label>
                            <Input type="month" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Week</label>
                            <Input type="week" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Time</label>
                            <Input type="time" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Color</label>
                            <Input type="color" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">File</label>
                            <Input type="file" name="" placeholder="Type here" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Checkbox</label>
                            <CustomInput type="checkbox" id="cb1" label="Checbox With Inline" inline />
                            <CustomInput type="checkbox" id="cb2" label="Checbox Without Inline" />
                        </FormGroup>
                    </Col>
                </Row>
            </div>
        </div>
    </Col>
</div>