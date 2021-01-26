<script>
    import { onMount } from "svelte";
    import { page, url, isActive } from "@roxi/routify";

    // Mount Jquery
    onMount(() => {
        go_jQuery();
    });

    // Start jQuery
    function go_jQuery() {
        !(function ($) {

            // Close Sidebar
            jQuery(document).on("click", ".close-sidebar", function(){
                jQuery(".cuba-app-sidebar").removeClass("collapse-mode");
                jQuery("header").removeClass("collapse-mode");
                jQuery("content").removeClass("collapse-mode");
            });

            // Sidebar Menu
            jQuery(document).on("click", ".sidebar-treeview", function(){
                if (!jQuery(this).parent(".sidebar-list").children(".sidebar-list-menu").hasClass("isOpen")){
                    jQuery(this).addClass("isOpen");
                    jQuery(this).children(".arrow").addClass("isOpen");
                    jQuery(this).parent(".sidebar-list").children(".sidebar-list-menu").addClass("isOpen");
                }
                else{
                    jQuery(this).removeClass("isOpen");
                    jQuery(this).children(".arrow").removeClass("isOpen");
                    jQuery(this).parent(".sidebar-list").children(".sidebar-list-menu").removeClass("isOpen");
                }
            });

        })(jQuery);
    }
</script>

<aside class="cuba-app-sidebar">
	<div class="logo">
        <img src="/images/logo-cuba.png" alt="Icon Application">
        <span class="close-sidebar">
            <div class="btn-container">
                <i class="material-icons">close</i>
                <span class="ripple-layer"></span>
            </div>
        </span>
	</div>
	<div class="main-content">
		<div class="sidebar-content">
            <ul class="sidebar-links">

                <!-- General -->
                <li class="sidebar-title">
                    <span class="title">General</span>
                    <span class="description">Global assets for apps</span>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/general/dashboard')}>
                    <a href={$url('/schema/general/dashboard')} class="list-content">
                        <span class="icon"><i class="material-icons">extension</i></span>
                        <span class="title">Dashboard</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/general/widgets')}>
                    <a href={$url('/schema/general/widgets')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Widgets</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/general/file-manager')}>
                    <a href={$url('/schema/general/file-manager')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">File Manager</span>
                    </a>
                </li>

                <!-- Forms -->
                <!-- UI Elements -->
                <li class="sidebar-title">
                    <span class="title">Forms</span>
                    <span class="description">Forms to build your apps</span>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/forms/form-elements')}>
                    <a href={$url('/schema/forms/form-elements')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Form Elements</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/forms/form-validation')}>
                    <a href={$url('/schema/forms/form-validation')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Form Validation</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/forms/form-editor')}>
                    <a href={$url('/schema/forms/form-editor')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Form Editor</span>
                    </a>
                </li>
    
                <!-- UI Elements -->
                <li class="sidebar-title">
                    <span class="title">UI Elements</span>
                    <span class="description">Elements to build your apps</span>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/card')}>
                    <a href={$url('/schema/ui-elements/card')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Card</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/typography')}>
                    <a href={$url('/schema/ui-elements/typography')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Typography</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/colors')}>
                    <a href={$url('/schema/ui-elements/colors')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Colors</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/buttons')}>
                    <a href={$url('/schema/ui-elements/buttons')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Buttons</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/alerts')}>
                    <a href={$url('/schema/ui-elements/alerts')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Alerts</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/notification')}>
                    <a href={$url('/schema/ui-elements/notification')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Notification</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/modal')}>
                    <a href={$url('/schema/ui-elements/modal')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Modal</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/badges')}>
                    <a href={$url('/schema/ui-elements/badges')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Badges</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/dropdown')}>
                    <a href={$url('/schema/ui-elements/dropdown')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Dropdown</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/jumbotron')}>
                    <a href={$url('/schema/ui-elements/jumbotron')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Jumbotron</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/breadcrumb')}>
                    <a href={$url('/schema/ui-elements/breadcrumb')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Breadcrumb</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/pagination')}>
                    <a href={$url('/schema/ui-elements/pagination')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Pagination</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/calendar')}>
                    <a href={$url('/schema/ui-elements/calendar')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Calendar</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/ui-elements/navigation')}>
                    <a href={$url('/schema/ui-elements/navigation')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Navigation</span>
                    </a>
                </li>
    
    
                <!-- Social Media -->
                <li class="sidebar-title">
                    <span class="title">Social Media</span>
                    <span class="description">Build your own social media</span>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/social-media/mailbox')}>
                    <a href={$url('/schema/social-media/mailbox')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Mailbox</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/social-media/chat')}>
                    <a href={$url('/schema/social-media/chat')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Chat</span>
                    </a>
                </li>
    
    
                <!-- E-commerce -->
                <li class="sidebar-title">
                    <span class="title">E-commerce</span>
                    <span class="description">Build your own online shop</span>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/product-homepage')}>
                    <a href={$url('/schema/e-commerce/product-homepage')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Product Homepage</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/products')}>
                    <a href={$url('/schema/e-commerce/products')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Products</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/product-detail')}>
                    <a href={$url('/schema/e-commerce/product-detail')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Product Detail</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/cart')}>
                    <a href={$url('/schema/e-commerce/cart')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Cart</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/invoice')}>
                    <a href={$url('/schema/e-commerce/invoice')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Invoice</span>
                    </a>
                </li>
                <li class="sidebar-list" class:active={$isActive('/schema/e-commerce/wishlist')}>
                    <a href={$url('/schema/e-commerce/wishlist')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Wishlist</span>
                    </a>
                </li>
    
    
                <!-- Pages -->
                <li class="sidebar-title">
                    <span class="title">Pages</span>
                    <span class="description">All Pages you can added</span>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/authentication/login')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Login</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/authentication/register')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Register</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/authentication/forgot-password')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Forgot Password</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/error/page_503')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">503</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/error/page_404')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">404</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href={$url('/schema/pages/error/page_403')} class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">403</span>
                    </a>
                </li>
                
    
                <!-- Multilevel -->
                <li class="sidebar-title">
                    <span class="title">Menu Level</span>
                    <span class="description">Create your own sidebar menu level</span>
                </li>
                <li class="sidebar-list">
                    <div class="list-content sidebar-treeview">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Level 2</span>
                        <span class="arrow"><i class="material-icons">chevron_left</i></span>
                    </div>
                    <ul class="sidebar-list-menu">
                        <li class="sidebar-list">
                            <a href={$url('/')} class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 2.1</span>
                            </a>
                        </li>
                        <li class="sidebar-list">
                            <a href={$url('/')} class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 2.2</span>
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="sidebar-list">
                    <div class="list-content sidebar-treeview">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Level 3</span>
                        <span class="arrow"><i class="material-icons">chevron_left</i></span>
                    </div>
                    <ul class="sidebar-list-menu">
                        <li class="sidebar-list">
                            <div class="list-content sidebar-treeview">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 3.1</span>
                                <span class="arrow"><i class="material-icons">chevron_left</i></span>
                            </div>
                            <ul class="sidebar-list-menu">
                                <li class="sidebar-list">
                                    <a href={$url('/')} class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.1</span>
                                    </a>
                                </li>
                                <li class="sidebar-list">
                                    <a href={$url('/')} class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.2</span>
                                    </a>
                                </li>
                            </ul>
                        </li>
                        <li class="sidebar-list">
                            <div class="list-content sidebar-treeview">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 3.2</span>
                                <span class="arrow"><i class="material-icons">chevron_left</i></span>
                            </div>
                            <ul class="sidebar-list-menu">
                                <li class="sidebar-list">
                                    <a href={$url('/')} class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.1</span>
                                    </a>
                                </li>
                                <li class="sidebar-list">
                                    <a href={$url('/')} class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.2</span>
                                    </a>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
    
            </ul>
        </div>
	</div>
</aside>