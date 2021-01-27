<script>
    import { onMount } from "svelte";
    import Icon from 'svelte-awesome';
    import { facebook, google, inbox, lock, mailForward, send, sendO, unlock, user } from 'svelte-awesome/icons';
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
        })(jQuery);
	}
</script>

<div class="auth-box">
    <div class="image-section">
        <img src="/images/auth-component/forgot-password-pict.png" alt="...">
    </div>
    <div class="content-section">
        <span class="pull-left full-width text-19 text-bold tcolor-normal mgb-10">Lupa Password</span>
        <span class="pull-left full-width text-14 tcolor-subtitle mgb-30">Silahkan masukkan data autentikasi anda pada form berikut.</span>
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
                    <span class="pull-left full-width text-14 tcolor-mid-normal mgb-5">Email</span>
                    <div class="cb-input-control">
                        <span class="icon-input-cb"><Icon data={inbox} /></span>
                        <input type="text" name="" class="input-cb" placeholder="Isikan disini">
                    </div>
                </div>
                <div class="pull-left full-width">
                    <div class="pull-left">
                        <button type="submit" class="btn-app bg-blue-light sm-btn">
                            Kirim Pergantian
                        </button>
                    </div>
                    <div class="pull-right">
                        <a href={$url("/schema/pages/authentication/login")} class="pull-left btn-app btn-outline-blue sm-btn" >
                            <i class="material-icons mgr-5">security</i> Login
                        </a>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>