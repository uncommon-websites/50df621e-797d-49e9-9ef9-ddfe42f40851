<section class="pt-20 pb-12 overflow-hidden">
	<div class="container-custom">
		<div class="max-w-4xl mb-12">
			<h1 class="text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight mb-4">
				The iOS terminal for AI-powered development
			</h1>
			<p class="text-2xl md:text-3xl text-muted font-light">
				Monitor your AI coding agents via SSH. <span class="text-accent">Get notified when they need you.</span>
			</p>
		</div>

		<div class="relative w-full aspect-[2/1] bg-black rounded-sm overflow-hidden group">
			<!-- Terminal Background -->
			<div class="absolute inset-0 bg-gradient-to-b from-gray-950 to-black"></div>
			
			<!-- Grid Pattern -->
			<div class="absolute inset-0 opacity-5" style="background-image: linear-gradient(rgba(255,255,255,0.1) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,0.1) 1px, transparent 1px); background-size: 20px 20px;"></div>
			
			<!-- Terminal Text Effect -->
			<div class="absolute inset-0 p-8 font-mono text-xs text-green-400/20 overflow-hidden leading-relaxed">
				<div class="space-y-1">
					<div>$ ssh user@dev-server</div>
					<div>Connected to dev-server</div>
					<div>$ tmux attach -t opencode</div>
					<div class="text-primary-400/30">→ AI agent running...</div>
					<div class="text-primary-400/30">→ Processing files...</div>
					<div class="text-primary-400/30">→ Waiting for input...</div>
				</div>
			</div>

			<!-- iPhone Mockup Frame -->
			<div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-64 h-[500px] bg-black rounded-[3rem] border-8 border-gray-900 shadow-2xl flex items-center justify-center">
				<!-- Screen -->
				<div class="w-full h-full bg-black rounded-[2.5rem] overflow-hidden relative">
					<!-- Status Bar -->
					<div class="absolute top-0 left-0 right-0 h-8 bg-gray-950 flex items-center justify-between px-6 text-white text-[8px]">
						<span>9:41</span>
						<div class="flex gap-1">
							<div class="w-3 h-2 border border-white rounded-[2px]"></div>
						</div>
					</div>
					
					<!-- Terminal Content -->
					<div class="absolute inset-0 top-8 bg-black p-3 font-mono text-[8px] text-green-400">
						<div class="space-y-1">
							<div class="text-gray-500">user@dev-server:~$</div>
							<div class="text-primary-400">→ opencode agent running</div>
							<div class="text-white">Analyzing codebase...</div>
							<div class="text-white">Making changes...</div>
							<div class="text-yellow-400 animate-pulse">⚠ Needs approval</div>
						</div>
					</div>
					
					<!-- Notification Badge -->
					<div class="absolute bottom-4 left-1/2 -translate-x-1/2 bg-white/95 backdrop-blur-sm px-3 py-1.5 rounded-full shadow-lg border border-gray-200 flex items-center gap-2 text-[8px] font-sans">
						<span class="w-2 h-2 bg-primary-500 rounded-full animate-pulse"></span>
						<span class="text-black font-medium">Agent needs input</span>
					</div>
				</div>
				
				<!-- Home Indicator -->
				<div class="absolute bottom-2 left-1/2 -translate-x-1/2 w-24 h-1 bg-white/20 rounded-full"></div>
			</div>
		</div>
	</div>
</section>
