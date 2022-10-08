<script lang="ts">
	let name: string = 'world';
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style lang="scss">

	@mixin mediaquery ($breakpoint) {
		@media screen and (max-width : $breakpoint) {
			@content;
		}
	}

	main {
		text-align : center;
		padding    : 1em;
		width  : 100%;
		margin     : 0 auto;
		background : steelblue;

		@include mediaquery(1024px) {
			width: 75%;
			background: blue;
		}

		h1 {
			color          : #ff3e00;
			text-transform : uppercase;
			font-size      : 4em;
			font-weight    : 100;
			color          : salmon;
		}
	}
</style>
