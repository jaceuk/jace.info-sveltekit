<script lang="ts">
	export let onClick: () => void;
</script>

<button class="button" on:click={onClick}>
	<slot />
</button>

<style lang="scss">
	button {
		color: var(--c-paper);
		border-radius: 200px;
		padding: var(--s-2) var(--s-3);
		border: 1px solid var(--c-nearly-accent);
		cursor: pointer;
		box-shadow: 0px 4px var(--s-1-2) var(--c-card-shadow);
		transition: var(--transition);
		width: fit-content;
		background: var(--c-accent);
		margin-left: auto;

		&:hover {
			background: var(--c-text);
		}
	}
</style>
