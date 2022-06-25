<script lang="ts">
	const pointers = [
		'cursor-auto',
		'cursor-default',
		'cursor-pointer',
		'cursor-wait',
		'cursor-text',
		'cursor-move',
		'cursor-help',
		'cursor-not-allowed',
		'cursor-none',
		'cursor-context-menu',
		'cursor-progress',
		'cursor-cell',
		'cursor-crosshair',
		'cursor-vertical-text',
		'cursor-alias',
		'cursor-copy',
		'cursor-no-drop',
		'cursor-grab',
		'cursor-grabbing',
		'cursor-all-scroll',
		'cursor-col-resize',
		'cursor-row-resize',
		'cursor-n-resize',
		'cursor-e-resize',
		'cursor-s-resize',
		'cursor-w-resize',
		'cursor-ne-resize',
		'cursor-nw-resize',
		'cursor-se-resize',
		'cursor-sw-resize',
		'cursor-ew-resize',
		'cursor-ns-resize',
		'cursor-nesw-resize',
		'cursor-nwse-resize',
		'cursor-zoom-in',
		'cursor-zoom-out'
	];
</script>

<main>
	<section class="grid grid-cols-1 md:grid-cols-4 gap-8 container mx-auto">
		{#each pointers as pointerClassName}
			<article class={`${pointerClassName} shadow-md text-center py-4 sm:py-4 md:py-12`}>
				{pointerClassName.replace('cursor-', '')}
			</article>
		{/each}
	</section>
</main>
