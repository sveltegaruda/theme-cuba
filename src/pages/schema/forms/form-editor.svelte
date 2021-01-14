<script>
    import { Col, Container, Row } from 'sveltestrap';
    import { quill } from 'svelte-quill'
    // import Editor from 'tailwind-editor'
    import Editor from 'cl-editor'
    
    let html = ''

    let options = { placeholder: "Write something from outside...", }
	
	let content = { html: '', text: ''};
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Form Editor</b></h4>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Summernote</b></h5>
            </div>
            <div class="card-body">
                Not Ready Yet ...
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Framework 7</b></h5>
            </div>
            <div class="card-body">
                Not Ready Yet ...
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Quill</b></h5>
                <span class="text-12">
                    See Documentation :
                    <a href="https://www.npmjs.com/package/svelte-quill">
                        <i>https://www.npmjs.com/package/svelte-quill</i>
                    </a>
                </span>
            </div>
            <div class="card-body">
                <div class="editor" use:quill={options} on:text-change={e => content = e.detail}/>
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>Tailwind Editor</b></h5>
                <span class="text-12">
                    See Documentation :
                    <a href="https://www.npmjs.com/package/tailwind-editor">
                        <i>https://www.npmjs.com/package/tailwind-editor</i>
                    </a>
                </span>
            </div>
            <div class="card-body">
                You can see example in <a href="https://editor-tw.fouita.com/?ref=madewithsvelte.com">https://editor-tw.fouita.com/?ref=madewithsvelte.com</a>
            </div>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title border-bottom-card">
                <h5><b>CL Editor</b></h5>
                <span class="text-12">
                    See Documentation :
                    <a href="https://github.com/nenadpnc/cl-editor">
                        <i>https://github.com/nenadpnc/cl-editor</i>
                    </a>
                </span>
            </div>
            <div class="card-body">
                <Editor />
            </div>
        </div>
    </Col>
</div>