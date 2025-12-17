<script lang="ts">
	import { onMount } from 'svelte';
	
	let showBanner = true;
</script>

{#if showBanner}
	<div class="bg-primary-50 border-b border-border py-2 px-4 text-xs font-mono flex justify-center items-center relative">
		<div class="flex items-center gap-2">
			<span class="text-muted">iOS only (for now). Join the TestFlight waitlist.</span>
			<a href="#waitlist" class="underline decoration-muted hover:text-accent transition-colors">Sign up.</a>
		</div>
		<button 
			class="absolute right-4 text-muted hover:text-foreground"
			aria-label="Close banner"
			onclick={() => showBanner = false}
		>
			<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M9 3L3 9M3 3L9 9" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
			</svg>
		</button>
	</div>
{/if}

<nav class="border-b border-border bg-background sticky top-0 z-50">
	<div class="container-custom h-16 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="text-xl font-bold tracking-tight flex items-center gap-2">
			<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-foreground">
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M9.61185 4.17065C8.2158 4.17065 6.92581 4.91543 6.22779 6.12444L3.72109 10.4662C3.02307 11.6752 3.02307 13.1647 3.72109 14.3737L6.22779 18.7155C6.92581 19.9245 8.2158 20.6693 9.61185 20.6693H14.6252C16.0213 20.6693 17.3113 19.9245 18.0093 18.7155L20.516 14.3737C21.214 13.1647 21.214 11.6752 20.516 10.4662L18.0093 6.12444C17.3113 4.91543 16.0213 4.17065 14.6252 4.17065H9.61185ZM14.6252 6.77569H11.4919C10.9905 6.77569 10.6773 7.31837 10.9283 7.75232C11.7029 9.09123 12.4793 10.4291 13.2527 11.7687C13.4854 12.1717 13.4854 12.6682 13.2527 13.0712C12.4793 14.4108 11.7029 15.7487 10.9283 17.0876C10.6773 17.5215 10.9905 18.0642 11.4919 18.0642H14.6252C15.0906 18.0642 15.5206 17.8159 15.7533 17.4129L18.26 13.0712C18.4927 12.6682 18.4927 12.1717 18.26 11.7687L15.7533 7.42695C15.5206 7.02395 15.0906 6.77569 14.6252 6.77569Z"
					fill="currentColor"
				/>
			</svg>
			<span class="font-sans font-semibold">ShellKey</span>
		</a>

		<!-- Links -->
		<div class="hidden md:flex items-center gap-8 font-mono text-xs text-muted">
			<a href="#features" class="hover:text-foreground transition-colors">Features</a>
			<a href="#download" class="hover:text-foreground transition-colors">Download</a>
		</div>

		<!-- CTA -->
		<div class="flex items-center gap-4">
			<a href="#waitlist" class="hidden md:flex items-center gap-2 border border-border px-3 py-1.5 text-xs font-mono hover:bg-primary-50 transition-colors uppercase">
				Join TestFlight
				<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M1 11L11 1M11 1H3M11 1V9" stroke="currentColor" stroke-width="1.5"/>
				</svg>
			</a>
			<div class="md:hidden">
				<!-- Mobile Menu Icon -->
				<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
					<line x1="3" y1="12" x2="21" y2="12"></line>
					<line x1="3" y1="6" x2="21" y2="6"></line>
					<line x1="3" y1="18" x2="21" y2="18"></line>
				</svg>
			</div>
		</div>
	</div>
</nav>
