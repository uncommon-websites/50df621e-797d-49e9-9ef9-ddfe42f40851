<section class="py-20 border-b border-border" id="download">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full" id="waitlist">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Get early access</p>
					<h2 class="text-2xl font-medium mb-4">Join the TestFlight waitlist</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						ShellKey is currently in private beta. Sign up to get notified when we open up TestFlight access. iOS only (for now).
					</p>
					<div class="flex gap-3 mb-12">
						<a href="#" class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							JOIN TESTFLIGHT
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">↗</span>
						</a>
					</div>
				</div>
				
				<!-- Terminal Visual -->
				<div class="mt-auto w-full h-48 bg-black relative overflow-hidden flex items-center justify-center font-mono">
					<!-- Terminal Lines -->
					<div class="absolute inset-0 p-4 text-green-400 text-[10px] leading-relaxed opacity-30">
						<div>$ ssh user@dev-server</div>
						<div>Connected to dev-server</div>
						<div>$ tmux attach -t opencode</div>
						<div class="text-primary-400">→ AI agent running...</div>
						<div class="text-primary-400">→ Monitoring for input...</div>
					</div>
					
					<!-- Centered Logo/Text -->
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-black/90 backdrop-blur-sm px-4 py-2 z-10 flex items-center gap-2 border border-primary-500/30">
							<svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-400">
								<path
									fill-rule="evenodd"
									clip-rule="evenodd"
									d="M9.61185 4.17065C8.2158 4.17065 6.92581 4.91543 6.22779 6.12444L3.72109 10.4662C3.02307 11.6752 3.02307 13.1647 3.72109 14.3737L6.22779 18.7155C6.92581 19.9245 8.2158 20.6693 9.61185 20.6693H14.6252C16.0213 20.6693 17.3113 19.9245 18.0093 18.7155L20.516 14.3737C21.214 13.1647 21.214 11.6752 20.516 10.4662L18.0093 6.12444C17.3113 4.91543 16.0213 4.17065 14.6252 4.17065H9.61185ZM14.6252 6.77569H11.4919C10.9905 6.77569 10.6773 7.31837 10.9283 7.75232C11.7029 9.09123 12.4793 10.4291 13.2527 11.7687C13.4854 12.1717 13.4854 12.6682 13.2527 13.0712C12.4793 14.4108 11.7029 15.7487 10.9283 17.0876C10.6773 17.5215 10.9905 18.0642 11.4919 18.0642H14.6252C15.0906 18.0642 15.5206 17.8159 15.7533 17.4129L18.26 13.0712C18.4927 12.6682 18.4927 12.1717 18.26 11.7687L15.7533 7.42695C15.5206 7.02395 15.0906 6.77569 14.6252 6.77569Z"
									fill="currentColor"
								/>
							</svg>
							<span class="text-white font-mono text-xs">ShellKey</span>
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Roadmap -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Coming soon</p>
				
				<div class="space-y-12">
					<!-- Roadmap 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Q1 2025</div>
						<div>
							<h3 class="font-medium text-sm mb-2">TestFlight Beta Launch</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Limited TestFlight beta for early adopters. Core features include SSH connectivity, Face ID authentication, tmux integration, and basic AI agent monitoring for OpenCode.
							</p>
							<span class="bg-primary-100 text-primary-700 text-[10px] px-1.5 py-0.5 rounded font-mono">In Progress</span>
						</div>
					</div>

					<!-- Roadmap 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Q2 2025</div>
						<div>
							<h3 class="font-medium text-sm mb-2">App Store Release</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Public App Store launch with expanded AI agent support for Claude Code and Cursor. Enhanced notification system with customizable triggers and improved terminal emulation.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Planned</span>
						</div>
					</div>

					<!-- Roadmap 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Q3 2025</div>
						<div>
							<h3 class="font-medium text-sm mb-2">Advanced Features</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Port forwarding, SFTP support, custom themes, and iPad optimization. Enhanced AI agent analytics and session recording capabilities.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Planned</span>
						</div>
					</div>

					<!-- Roadmap 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">Future</div>
						<div>
							<h3 class="font-medium text-sm mb-2">Cross-Platform Expansion</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Android support and potential desktop companion app. Built on React Native/Expo foundation for seamless cross-platform deployment.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Exploring</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>
