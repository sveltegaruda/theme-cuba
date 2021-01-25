<script>
    import { onMount } from "svelte";
    import Icon from 'svelte-awesome';
    import { facebook, google, lock, send, sendO, unlock, user } from 'svelte-awesome/icons';
    import { page, url, isActive } from "@roxi/routify";

    // Mount Jquery
    onMount(() => {
        go_jQuery();
    });

    // Start jQuery
    function go_jQuery() {
        !(function ($) {
            // *
            // Set Input Application
            // *
                jQuery(".input-cb").blur(function(){
                    jQuery(this).parent(".cb-input-control").removeClass("isFocused");
                    jQuery(this).parent(".cb-input-control").children(".icon-input-cb").removeClass("isFocused");
                }).focus(function(){
                    jQuery(this).parent(".cb-input-control").addClass("isFocused");
                    jQuery(this).parent(".cb-input-control").children(".icon-input-cb").addClass("isFocused");
                });

                jQuery(document).on("click", ".cb-input-control", function(){
                    jQuery(this).children(".input-cb").focus();
                });
            // ----------------- End --------------------

            // *
            // Set Input Password
            // *
                jQuery(document).on("click", ".i-pass", function(){
                    if(!jQuery(this).children(".locked").hasClass("visible")){

                        jQuery(this).children(".locked").removeClass("hidden");
                        jQuery(this).children(".locked").addClass("visible");
                        jQuery(this).children(".unlocked").removeClass("visible");
                        jQuery(this).children(".unlocked").addClass("hidden");
                        jQuery(this).parent(".cb-input-control").children("input").attr("type", "password");
                    }
                    else{
                        jQuery(this).children(".locked").removeClass("visible");
                        jQuery(this).children(".locked").addClass("hidden");
                        jQuery(this).children(".unlocked").removeClass("hidden");
                        jQuery(this).children(".unlocked").addClass("visible");
                        jQuery(this).parent(".cb-input-control").children("input").attr("type", "text");
                    }
                });
            // ----------------- End --------------------
        })(jQuery);
	}
</script>

<div class="auth-box">
    <div class="image-section">
        <!-- <img src="/images/auth-component/" alt="Load image..." /> -->
        <img src="/images/auth-component/login-pict.png" alt="...">
    </div>
    <div class="content-section">
        <span class="pull-left full-width text-19 text-bold tcolor-normal mgb-10">Login</span>
        <span class="pull-left full-width text-14 tcolor-subtitle mgb-30">Silahkan masukkan akun anda pada form berikut.</span>
        <div class="pull-left full-width mgb-30">
            <form action="./" method="POST" enctype="multipart/form-data">
                <div class="pull-left full-width">
                    <span class="pull-left full-width text-14 tcolor-mid-normal mgb-5">Username</span>
                    <div class="cb-input-control">
                        <span class="icon-input-cb"><Icon data={user} /></span>
                        <input type="text" name="" class="input-cb" placeholder="Isikan disini">
                    </div>
                </div>
                <div class="pull-left full-width">
                    <span class="pull-left full-width text-14 tcolor-mid-normal mgb-5">Password</span>
                    <div class="cb-input-control">
                        <span id="passTooltip" class="icon-input-cb i-pass">
                            <span class="locked visible">
                                <Icon data={ lock } />
                            </span>
                            <span class="unlocked hidden">
                                <Icon data={ unlock } />
                            </span>
                        </span>
                        <input type="text" name="" class="input-cb" placeholder="Isikan disini">
                    </div>
                </div>
                <div class="pull-left full-width mgb-10">
                    <div class="pull-right">
                        <a href="{$url('/schema/pages/authentication/forgot-password')}" class="text-14">Lupa Password?</a>
                    </div>
                </div>
                <div class="pull-left full-width">
                    <div class="pull-left">
                        <button type="submit" class="btn-app bg-blue sm-btn">
                            <Icon data={ send } class="mgr-5" /> Login
                        </button>
                    </div>
                    <div class="pull-right">
                        <a href="{$url('/schema/pages/authentication/register')}" type="submit" class="pull-left btn-app btn-outline-red sm-btn">Daftar Akun</a>
                    </div>
                </div>
            </form>
        </div>
        <div class="pull-right full-width">
            <div class="component-devider">
                <span class="line-gate"></span>
                <span class="text">Atau</span>
                <span class="line-gate"></span>
            </div>
            <div class="pull-left full-width mgt-20 df-fdr df-algn-jtfct-ct">
                <a href="./" class="btn-app bg-blue xs-btn mgr-10">
                    <Icon data={ facebook }  class="text-17 mgr-5" /> Facebook
                </a>
                <a href="./" class="btn-app bg-red xs-btn">
                    <Icon data={ google }  class="text-17 mgr-5" /> Google
                </a>
            </div>
        </div>
    </div>
</div>