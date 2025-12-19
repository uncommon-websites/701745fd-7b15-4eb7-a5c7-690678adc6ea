<script lang="ts">
	import { page } from "$app/state";
</script>

<div class="min-h-screen bg-white text-black font-sans px-6 py-8 md:px-10 md:py-10 flex items-center justify-center">
	<div class="max-w-2xl text-center">
		<h1 class="text-[64px] md:text-[96px] font-light mb-4">{page.status}</h1>
		<p class="text-[20px] md:text-[24px] text-gray-600 mb-8">
			{page.error?.message ?? "This moment seems to have slipped away."}
		</p>
		<p class="text-[15px] text-gray-400 italic mb-8">
			一期一会 — Even errors are fleeting moments.
		</p>
		<a 
			href="/" 
			class="inline-block px-6 py-3 bg-black text-white text-[15px] hover:bg-gray-800 transition-colors"
		>
			Return Home
		</a>
	</div>
</div>
