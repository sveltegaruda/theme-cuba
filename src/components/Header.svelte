<script>
	import { onMount } from "svelte";
	import Icon from 'svelte-awesome';
	import { angleDown, circleO, user } from 'svelte-awesome/icons';
	// import Fullscreen from "svelte-fullscreen";

    // Mount Jquery
    onMount(() => {
        go_jQuery();
    });

    // Start jQuery
    function go_jQuery() {
        !(function ($) {

			// Toggle Sidebar
			jQuery(document).on('click', ".toggle-sidebar", function() {
				if (!jQuery("header").hasClass("collapse-mode")) {
					jQuery(".cuba-app-sidebar").addClass("collapse-mode");
					jQuery("header").addClass("collapse-mode");
					jQuery("content").addClass("collapse-mode");
				}
				else{
					jQuery(".cuba-app-sidebar").removeClass("collapse-mode");
					jQuery("header").removeClass("collapse-mode");
					jQuery("content").removeClass("collapse-mode");
				}
			});

			// Dropdown
			jQuery(document).on('click', ".toggle-dropdown", function() {
				jQuery(".toggle-dropdown").not(jQuery(this)).parent().children(".dropdown-app").removeClass("isOpen");
				if (!jQuery(this).parent().children(".dropdown-app").hasClass("isOpen")){
					jQuery(this).parent().children(".dropdown-app").addClass("isOpen");
				}
				else{
					jQuery(this).parent().children(".dropdown-app").removeClass("isOpen");
				}
				return false;
			});

			jQuery(document).on("click", ".dropdown-app", function(){
				jQuery(this).addClass("isOpen");
				return false;
			});

			jQuery(document).on("click", function(e){
				if (!jQuery(this).hasClass(".toggle-dropdown") || !jQuery(this).hasClass("dropdown-app")){
					jQuery(".toggle-dropdown").not(jQuery(this)).parent().children(".dropdown-app").removeClass("isOpen");
				}
			});

        })(jQuery);
	}
</script>

<header>
	<div class="main-header">
		<!-- <span class="toggle-sidebar" on:click={sidebarToggle}> -->
		<span class="toggle-sidebar">
			<i class="material-icons">sort</i>
			<span class="ripple-layer"></span>
		</span>
		<form class="form-search">
			<input type="text" name="" placeholder="Search...">
			<button><i class="material-icons">search</i></button>
		</form>
		<div class="header-container">
			<ul>
				<li>
					<i class="main-icon toggle-dropdown material-icons">notifications_none</i>
					<span class="sirens sirens-green"></span>
					<div class="dropdown-app lg-dropdown">
						<div class="header-dropdown">
							<span class="title">Notification</span>
							<span class="icon"><i class="material-icons">notifications_none</i></span>
						</div>
						<div class="content-dropdown">
							<ul class="dropdown-notification-list">
								<li>
									<a href="./">
										<div class="description">
											<Icon data={circleO} class="font-primary mgr-5" />
											<span class="context">Delivery Processing</span>
										</div>
										<div class="update-time">10 Min</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="description">
											<Icon data={circleO} class="font-danger mgr-5" />
											<span class="context">Order Complete</span>
										</div>
										<div class="update-time">10 Min</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="description">
											<Icon data={circleO} class="font-info mgr-5" />
											<span class="context">Tickets Generated</span>
										</div>
										<div class="update-time">10 Min</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="description">
											<Icon data={circleO} class="font-success mgr-5" />
											<span class="context">Delivery Complete</span>
										</div>
										<div class="update-time">10 Min</div>
									</a>
								</li>
							</ul>
						</div>
						<div class="footer-dropdown">
							<a href="./" class="full-width btn-app xs-btn bg-blue">Check All Notification</a>
						</div>
					</div>
				</li>
				<li>
					<i class="main-icon toggle-dropdown material-icons">chat</i>
					<span class="nav-unread badge badge-danger sirens-red sirens-red">3</span>
					<div class="dropdown-app lg-dropdown">
						<div class="header-dropdown">
							<span class="title">Messages</span>
							<span class="icon"><i class="material-icons">chat_bubble_outline</i></span>
						</div>
						<div class="content-dropdown">
							<ul class="dropdown-message-list">
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Febima H. H.</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Danang Dandies</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Febima H. H.</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Danang Dandies</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Febima H. H.</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
								<li>
									<a href="./">
										<div class="image">
											<img src="./assets/images/avatar.jpg" alt="...">
										</div>
										<div class="list-content">
											<div class="sender">
												<span class="sender-name">Danang Dandies</span>
												<span class="time-send tcolor-green">05 Jan 2021</span>
											</div>
											<div class="description">This is dummy data messages for Start Up</div>
										</div>
									</a>
								</li>
							</ul>
						</div>
						<div class="footer-dropdown">
							<a href="./" class="full-width btn-app xs-btn bg-blue">View All Messages</a>
						</div>
					</div>
				</li>
				<!-- <li>
					<i class="main-icon material-icons">center_focus_weak</i>
				</li> -->
				<li>
					<div class="avatar-header toggle-dropdown">
						<img src="./assets/images/avatar.jpg" alt="...">
						<div class="bio">
							<div class="name">Svelte Garuda</div>
							<div class="status">Maintainer <Icon data={angleDown}/></div>
						</div>
					</div>
					<div class="dropdown-app sm-dropdown">
						<div class="content-dropdown">
							<ul class="dropdown-user-list">
								<li>
									<a href="./">
										<span class="icon"><i class="material-icons">person_outline</i></span>
										<span class="description">Profile</span>
									</a>
								</li>
								<li>
									<a href="./">
										<span class="icon"><i class="material-icons">mail_outline</i></span>
										<span class="description">Inbox</span>
									</a>
								</li>
								<li>
									<a href="./">
										<span class="icon"><i class="material-icons">insert_chart_outlined</i></span>
										<span class="description">Taskboard</span>
									</a>
								</li>
								<li>
									<a href="./">
										<span class="icon"><i class="material-icons">settings</i></span>
										<span class="description">Settings</span>
									</a>
								</li>
								<li>
									<a href="./">
										<span class="icon"><i class="material-icons">login</i></span>
										<span class="description">Logout</span>
									</a>
								</li>
							</ul>
						</div>
					</div>
				</li>
			</ul>
		</div>
	</div>
</header>