<div class="overlay"><slot /></div>

<style lang="scss">
	.overlay {
		width: 100%;
		height: 100%;
		position: fixed;
		background: rgba(0, 0, 0, 0.6);
		top: 0;
		left: 0;
		right: 0;
		z-index: 100;
		display: flex;
		align-items: center;
		justify-content: center;
		animation: mmfadeIn 0.2s ease-in-out;
		z-index: 1000;

		@keyframes mmfadeIn {
			from {
				opacity: 0;
			}

			to {
				opacity: 1;
			}
		}
	}
</style>
