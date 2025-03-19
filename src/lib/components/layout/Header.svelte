<script>
    import { Navigation } from '@skeletonlabs/skeleton-svelte';
    import logo from '$lib/assets/images/W_N_SVG_ClypperLogo.svg';
</script>

<header class="sticky top-0 z-10 header">
    <div class="header-inner-wrapper">
        <div class="logo-title-wrapper">
            <img src={logo} width=65 height=65 alt="Clypper Technology Logo">
            <div class="title-wrapper">
                <h3 class="h3">Clypper's</h3>
                <h4 class="h4">Backlog</h4>
            </div>
        </div>
        <div class="nav-wrapper">
            <Navigation.Bar height="">
                <Navigation.Tile label="Customers" href="customers"/>
                <Navigation.Tile label="Backlog" href="backlog" />
            </Navigation.Bar>
        </div>


    </div>
</header>               

<style>
    .header {
        display: flex;
        flex-direction: row;
        justify-content: center;
        padding: 20px 0;
    }

    .header-inner-wrapper {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        justify-content: space-between;
        align-items: center;
        max-width: 1080px;
        width: 100%;
        padding: 0 20px;
    }

    .logo-title-wrapper {
        display: flex;
        gap: 5px;
    }
</style>