<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';
	let { data, children } = $props();
</script>

<div class="h-screen flex flex-col overflow-hidden">
	<Navbar {data} />
	<div class="flex-1 overflow-hidden">
		{@render children()}
	</div>
</div>
