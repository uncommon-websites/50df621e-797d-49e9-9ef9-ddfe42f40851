<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: SSH from your iPhone -->
<FeatureBlock 
	title="SSH from your iPhone" 
	description="Full-featured terminal emulation with custom libssh2 implementation. Connect to your dev servers from anywhere."
	buttons={[
		{ text: "JOIN TESTFLIGHT", icon: true }
	]}
>
	<div class="w-full h-full bg-black border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-gray-800 pb-2 mb-4">
			<span class="text-primary-400">$</span>
			<span class="text-gray-400">user@dev-server:~</span>
			<span class="w-2 h-4 bg-primary-400 animate-pulse"></span>
		</div>
		<div class="space-y-2 text-green-400">
			<div>$ ssh user@production</div>
			<div class="text-gray-500">Connected to production</div>
			<div>$ tmux attach -t main</div>
			<div class="text-primary-400">→ Session restored</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: AI Agent Notifications -->
<FeatureBlock 
	title="Get notified when agents need you" 
	description="Built-in monitoring for OpenCode, Claude Code, and Cursor. Receive push notifications when your AI agent is waiting for input."
	buttons={[
		{ text: "LEARN MORE", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-primary-500 rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-primary-500 rounded-[1px] animate-pulse"></div>
			</div>
			Monitoring AI agent...
		</div>
		<div class="w-full bg-gray-100 h-1.5 rounded-full overflow-hidden">
			<div class="bg-primary-500 h-full w-2/3"></div>
		</div>
		<div class="flex gap-1">
			{#each Array(20) as _, i}
				<div class="w-1 h-3 {i < 14 ? 'bg-primary-200' : 'bg-gray-200'}"></div>
			{/each}
		</div>
		<div class="mt-2 p-3 bg-primary-50 border border-primary-200 rounded flex items-center gap-2 text-xs font-mono">
			<span class="text-primary-600">⚠</span>
			<span class="text-primary-900">Agent needs approval</span>
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Face ID Security -->
<FeatureBlock 
	title="Face ID protected SSH keys" 
	description="Your SSH keys are stored in the iOS Secure Enclave and protected by biometric authentication. They never leave your device."
	buttons={[
		{ text: "LEARN ABOUT SECURITY", icon: true }
	]}
>
	<div class="w-full h-full bg-gradient-to-br from-gray-50 to-white border border-border rounded shadow-sm overflow-hidden flex items-center justify-center p-8">
		<div class="flex flex-col items-center gap-6">
			<!-- Face ID Icon -->
			<div class="w-20 h-20 rounded-full bg-primary-100 flex items-center justify-center">
				<svg width="40" height="40" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-600">
					<circle cx="12" cy="12" r="10" stroke="currentColor" stroke-width="2"/>
					<circle cx="9" cy="10" r="1.5" fill="currentColor"/>
					<circle cx="15" cy="10" r="1.5" fill="currentColor"/>
					<path d="M9 15C9 15 10 17 12 17C14 17 15 15 15 15" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
				</svg>
			</div>
			
			<!-- Security Badge -->
			<div class="flex flex-col items-center gap-2">
				<div class="px-3 py-1 bg-primary-600 text-white text-xs font-mono rounded-full">
					SECURE ENCLAVE
				</div>
				<div class="text-xs text-muted font-mono text-center">
					Biometric authentication required
				</div>
			</div>
			
			<!-- Key Icon -->
			<div class="flex items-center gap-2 text-xs font-mono text-muted">
				<svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-500">
					<path d="M7 10V7C7 4.23858 9.23858 2 12 2C14.7614 2 17 4.23858 17 7V10M12 14V17M5 10H19C20.1046 10 21 10.8954 21 12V20C21 21.1046 20.1046 22 19 22H5C3.89543 22 3 21.1046 3 20V12C3 10.8954 3.89543 10 5 10Z" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
				</svg>
				<span>Keys never leave device</span>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 4: Seamless Reconnection -->
<FeatureBlock 
	title="Seamless reconnection with tmux" 
	description="Built-in tmux session persistence means you pick up exactly where you left off. No lost work, no context switching."
	buttons={[
		{ text: "SEE IT IN ACTION", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-black border border-border rounded shadow-sm overflow-hidden font-mono text-[10px] p-4">
		<div class="space-y-3 text-green-400">
			<div class="flex items-center gap-2 text-gray-500">
				<span class="text-primary-400">→</span>
				<span>Connection lost</span>
			</div>
			<div class="h-px bg-gray-800 my-2"></div>
			<div class="flex items-center gap-2">
				<span class="text-primary-400">→</span>
				<span>Reconnecting...</span>
			</div>
			<div class="flex items-center gap-2">
				<span class="text-primary-400">✓</span>
				<span>Connected</span>
			</div>
			<div class="flex items-center gap-2">
				<span class="text-primary-400">✓</span>
				<span>tmux session restored</span>
			</div>
			<div class="h-px bg-gray-800 my-2"></div>
			<div class="text-gray-400">
				<div>$ vim src/main.rs</div>
				<div class="text-gray-600 mt-2"># Your work is exactly as you left it</div>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 5: OpenCode Integration -->
<FeatureBlock 
	title="Built-in OpenCode support" 
	description="Native integration with opencode server monitoring. Track your AI coding sessions and respond to prompts instantly."
	buttons={[
		{ text: "LEARN MORE", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-2">
			<div class="text-[10px] font-mono text-muted flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
				opencode.ai session active
			</div>
		</div>
		
		<!-- Activity Timeline -->
		<div class="space-y-2">
			<div class="flex items-start gap-2 text-[10px] font-mono">
				<span class="text-primary-500 mt-0.5">→</span>
				<div class="flex-1">
					<div class="text-foreground">Analyzing codebase</div>
					<div class="text-gray-400">2 min ago</div>
				</div>
			</div>
			<div class="flex items-start gap-2 text-[10px] font-mono">
				<span class="text-primary-500 mt-0.5">→</span>
				<div class="flex-1">
					<div class="text-foreground">Generated changes</div>
					<div class="text-gray-400">1 min ago</div>
				</div>
			</div>
			<div class="flex items-start gap-2 text-[10px] font-mono">
				<span class="text-yellow-500 mt-0.5">⚠</span>
				<div class="flex-1">
					<div class="text-foreground font-semibold">Waiting for approval</div>
					<div class="text-gray-400">Just now</div>
				</div>
			</div>
		</div>

		<div class="mt-auto">
			<div class="bg-primary-50 p-3 rounded border border-primary-200 flex gap-2 items-center text-[10px] font-mono">
				<div class="w-4 h-4 bg-primary-500 rounded flex items-center justify-center text-white text-[8px]">!</div>
				<div class="text-primary-900">Notification sent to iPhone</div>
			</div>
		</div>
	</div>
</FeatureBlock>
