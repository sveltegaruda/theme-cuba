<script>
    import { onMount } from "svelte";

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
            jQuery(document).on("click", ".list-content", function(){
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

            // Custom Scrollbar
            var el = document.querySelector('.custom-scrollbar');
            SimpleScrollbar.initEl(el);

        })(jQuery);
    }
</script>

<aside class="cuba-app-sidebar">
	<div class="logo">
        <img src="./assets/images/logo-cuba.png" alt="">
        <span class="close-sidebar">
            <div class="btn-container">
                <i class="material-icons">close</i>
                <span class="ripple-layer"></span>
            </div>
        </span>
	</div>
	<div class="main-content">
		<div class="sidebar-content custom-scrollbar">
            <ul class="sidebar-links">

                <!-- General -->
                <li class="sidebar-title">
                    <span class="title">General</span>
                    <span class="description">Global assets for apps</span>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">extension</i></span>
                        <span class="title">Dashboard</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Widgets</span>
                    </a>
                </li>
    
                <!-- Component -->
                <li class="sidebar-title">
                    <span class="title">Component</span>
                    <span class="description">Component to build your apps</span>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Card</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Notification</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Modals</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Calendar</span>
                    </a>
                </li>
    
                <!-- UI Elements -->
                <li class="sidebar-title">
                    <span class="title">UI Elements</span>
                    <span class="description">Elements to build your apps</span>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Typography</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Alerts</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Buttons</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Dropdown</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Colors</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Pagination</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Navigation</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Breadcrumb</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Badges</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Jumbotron</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Panels</span>
                    </a>
                </li>
    
    
                <!-- UI Elements -->
                <li class="sidebar-title">
                    <span class="title">Email & Chat</span>
                    <span class="description">Build your own social media</span>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Email</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Chat</span>
                    </a>
                </li>
    
    
                <!-- E-commerce -->
                <li class="sidebar-title">
                    <span class="title">E-commerce</span>
                    <span class="description">Build your own online shop</span>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Product Homepage</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Products</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Product Detail</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Cart</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
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
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Login</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Register</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Forgot Password</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">503</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">404</span>
                    </a>
                </li>
                <li class="sidebar-list">
                    <a href="./" class="list-content">
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
                    <div class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Level 2</span>
                        <span class="arrow"><i class="material-icons">chevron_left</i></span>
                    </div>
                    <ul class="sidebar-list-menu">
                        <li class="sidebar-list">
                            <a href="./" class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 2.1</span>
                            </a>
                        </li>
                        <li class="sidebar-list">
                            <a href="./" class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 2.2</span>
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="sidebar-list">
                    <div class="list-content">
                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                        <span class="title">Level 3</span>
                        <span class="arrow"><i class="material-icons">chevron_left</i></span>
                    </div>
                    <ul class="sidebar-list-menu">
                        <li class="sidebar-list">
                            <div class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 3.1</span>
                                <span class="arrow"><i class="material-icons">chevron_left</i></span>
                            </div>
                            <ul class="sidebar-list-menu">
                                <li class="sidebar-list">
                                    <a href="./" class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.1</span>
                                    </a>
                                </li>
                                <li class="sidebar-list">
                                    <a href="./" class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.2</span>
                                    </a>
                                </li>
                            </ul>
                        </li>
                        <li class="sidebar-list">
                            <div class="list-content">
                                <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                <span class="title">Level 3.2</span>
                                <span class="arrow"><i class="material-icons">chevron_left</i></span>
                            </div>
                            <ul class="sidebar-list-menu">
                                <li class="sidebar-list">
                                    <a href="./" class="list-content">
                                        <span class="icon"><i class="material-icons">drag_indicator</i></span>
                                        <span class="title">Level 1.1</span>
                                    </a>
                                </li>
                                <li class="sidebar-list">
                                    <a href="./" class="list-content">
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