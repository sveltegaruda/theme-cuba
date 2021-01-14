<script>
    import {
        Col,
        FormGroup,
        Input,
        InputGroup,
        InputGroupAddon,
        InputGroupText,
        CustomInput,
        Row
    } from 'sveltestrap';
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Form Validation</b></h4>
        </div>
    </Col>
    <Col md="12">
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Form Validation</b></h5>
                <p class="text-12">
                    For Custom Bootstrap form validation messages, to giving notification for every validation.
                </p>
            </div>
            <div class="card-body">
                <Row>
                    <Col md="4">
                        <FormGroup>
                            <label for="">First Name</label>
                            <Input text="text" name="" placeholder="First Name" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Last Name</label>
                            <Input text="text" name="" placeholder="Last Name" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Username</label>
                            <InputGroup>
                                <InputGroupAddon addonType="prepend">
                                    <InputGroupText>@</InputGroupText>
                                </InputGroupAddon>
                                <Input placeholder="username" />
                            </InputGroup>
                        </FormGroup>
                    </Col>
                </Row>
                <Row>
                    <Col md="6">
                        <FormGroup>
                            <label for="">City</label>
                            <Input text="text" name="" placeholder="City" />
                        </FormGroup>
                    </Col>
                    <Col md="3">
                        <FormGroup>
                            <label for="">State</label>
                            <Input text="text" name="" placeholder="State" />
                        </FormGroup>
                    </Col>
                    <Col md="3">
                        <FormGroup>
                            <label for="">Zip</label>
                            <Input text="text" name="" placeholder="Zip" />
                        </FormGroup>
                    </Col>
                </Row>
                <Row>
                    <Col md="12">
                        <div>
                            <CustomInput type="checkbox" id="exampleCustomInline" label="Agree to terms and conditions" inline />
                        </div>
                    </Col>
                    <Col md="12">
                        <div class="mgt-15">
                            <button class="btn-app bg-blue">Submit Form</button>
                        </div>
                    </Col>
                </Row>
            </div>
        </div>
    </Col>
</div>