<script>
    import Sidebar from "./defaults/Sidebar.svelte";
    import Header from "./defaults/Header.svelte";
    import Footer from "./defaults/Footer.svelte";

</script>
<!-- routify:options preload="proximity" -->

<Sidebar/>
<Header/>
<content>
    <!-- Slot -->
    <slot />

    <!-- Footer -->
    <Footer/>
</content>
