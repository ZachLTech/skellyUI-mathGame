<script>
    import '@skeletonlabs/skeleton/themes/theme-crimson.css';
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	import '../app.postcss';
	import { AppBar } from '@skeletonlabs/skeleton';
	import logo from '$lib/assets/logo.png';
    import { AppShell } from '@skeletonlabs/skeleton';
</script>


<AppShell regionPage="relative" slotPageHeader="hide-scrollbar sticky top-0 z-10">
	<svelte:fragment slot="header">
        <AppBar>
            <svelte:fragment slot="lead">
                <img width="60" src={logo} alt="LOGO">
            </svelte:fragment>
            <svelte:fragment slot="trail">
                <a
                    class="btn btn-lg variant-ghost-primary"
                    href="#"
                    rel="noreferrer"
                >
                    <strong>Start</strong>
                </a>
            </svelte:fragment>
        </AppBar>
    </svelte:fragment>

    <svelte:fragment>
        <slot />
    </svelte:fragment>
    
</AppShell>