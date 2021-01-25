<script>
    import {
        Col,
        FormGroup,
        Label,
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
                            <Label for="exampleCustomFileBrowser">File Browser</Label>
                            <CustomInput type="file" id="exampleCustomFileBrowser" name="customFile" label="Pick a File" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <Label for="exampleCustomSelect">Custom Select</Label>
                            <CustomInput type="select" id="exampleCustomSelect" name="customSelect">
                                <option value="">Select</option>
                                <option>Value 1</option>
                                <option>Value 2</option>
                                <option>Value 3</option>
                                <option>Value 4</option>
                                <option>Value 5</option>
                            </CustomInput>
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <Label for="exampleCustomSelectDisabled">Custom Select Disabled</Label>
                            <CustomInput type="select" id="exampleCustomSelectDisabled" name="customSelect" disabled>
                                <option value="">Select</option>
                                <option>Value 1</option>
                                <option>Value 2</option>
                                <option>Value 3</option>
                                <option>Value 4</option>
                                <option>Value 5</option>
                            </CustomInput>
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Checkbox</label>
                            <CustomInput type="checkbox" id="cb1" label="Checbox Inline 1" inline />
                            <CustomInput type="checkbox" id="cb2" label="Checbox Inline 2" inline />
                            <CustomInput type="checkbox" id="cb3" label="Checbox Disabled 1" inline disabled />
                            <CustomInput type="checkbox" id="cb4" label="Checbox Disabled 2" inline disabled />
                            <CustomInput type="checkbox" id="cb5" label="Checbox Without Inline" />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Radio Button</label>
                            <CustomInput type="radio" id="exampleCustomRadio" name="customRadio" label="Select this custom radio" />
                            <CustomInput type="radio" id="exampleCustomRadio2" name="customRadio" label="Or this one" />
                            <CustomInput type="radio" id="exampleCustomRadio3" label="But not this disabled one" disabled />
                            <CustomInput type="radio" id="exampleCustomRadio4" label="Can't click this label to select!" htmlFor="exampleCustomRadio4_X" disabled />
                        </FormGroup>
                    </Col>
                    <Col md="4">
                        <FormGroup>
                            <label for="">Switches</label>
                            <CustomInput type="switch" id="exampleCustomSwitch" name="customSwitch" label="Turn on this custom switch" />
                            <CustomInput type="switch" id="exampleCustomSwitch2" name="customSwitch" label="Or this one" />
                            <CustomInput type="switch" id="exampleCustomSwitch3" label="But not this disabled one" disabled />
                            <CustomInput type="switch" id="exampleCustomSwitch4" label="Can't click this label to turn on!" htmlFor="exampleCustomSwitch4_X" disabled />
                        </FormGroup>
                    </Col>
                </Row>
            </div>
        </div>
    </Col>
</div>