<script>
    import { onMount } from "svelte";
    import { Col, Container, Row } from 'sveltestrap';
    import Prism from "./PrismJS.svelte";

    // Create Code With Prism JS
    let html_code = `
        <button class="btn-app bg-blue mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="primary" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
            Primary
        </button>
        <button class="btn-app bg-teal mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="info" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
            Info
        </button>
        <button class="btn-app bg-orange mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="warning" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
            Warning
        </button>
        <button class="btn-app bg-red" data-widget="notify" data-from="bottom" data-align="right" data-type="danger" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
            Danger
        </button>
    `;

    // Mount Jquery
    onMount(() => {
        go_jQuery();
    });

    // Start jQuery
    function go_jQuery() {
        !(function ($) {

            function showNotification(from, align, type, msg) {
                // type = ['', 'info', 'danger', 'success', 'warning', 'rose', 'primary'];
                $.notify(
                    {
                        icon        : "error_outline", //Material Icons
                        message     : msg
                    },
                    {
                        type        : type,
                        delay       : 5000,
                        timer       : 3000,
                        placement   : {
                            from        : from,
                            align       : align
                        }
                    }
                );
            }

            jQuery(document).on("click", "[data-widget='notify']", function(){
                let from = jQuery(this).data('from');
                let align = jQuery(this).data('align');
                let type = jQuery(this).data('type');
                let msg = jQuery(this).data('msg');

                showNotification(from, align, type, msg);
            });

        })(jQuery);
    }
</script>
<div class="cuba-app-content">
    <Col md="12">
        <div class="pull-left full-width pdt-30 pdb-30">
            <h4><b>Notification</b></h4>
        </div>
    </Col>
    <Col md=12>
        <div class="card pda-30">
            <div class="card-title">
                <h5><b>In your HTML components</b></h5>
                <p class="text-12">You can add this component to your HTML, include <code>data-[widget, from, align, type]</code> to your component to call it.</p>
                <Prism language="r" code="{html_code}" header="Example Code"/>
            </div>
            <div class="card-body">
                <button class="btn-app bg-blue mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="primary" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
                    Primary
                </button>
                <button class="btn-app bg-teal mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="info" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
                    Info
                </button>
                <button class="btn-app bg-orange mgr-10" data-widget="notify" data-from="bottom" data-align="right" data-type="warning" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
                    Warning
                </button>
                <button class="btn-app bg-red" data-widget="notify" data-from="bottom" data-align="right" data-type="danger" data-msg="<b>Attention</b> - This is notification by Bootstrap Notify Growl Like">
                    Danger
                </button>
            </div>
        </div>
    </Col>
</div>