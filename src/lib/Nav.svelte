<script>
	import Icon from 'svelte-awesome';
	import { faHome } from '@fortawesome/free-solid-svg-icons';
	import { fade } from 'svelte/transition';
</script>

<div>
	<div class="icon-container">
		<a href="/" class="link-button"
			><Icon data={faHome} scale="2" /> <span transition:fade>Home</span></a
		>
	</div>
	<a href="/about">About</a>
	<a href="/work">Work</a>
</div>

<style>
	.icon-container {
		background-color: var(--dark-gray);
		padding: 8px;
		max-width: fit-content;
		border-radius: 25px;
		box-shadow: 1px 1px 10px hsla(0, 0%, 0%, 0.25);
	}

	.link-button {
		color: var(--light-gray);
	}

	.link-button:hover {
		color: var(--green);
	}

	.link-button > span {
		display: none;
	}

	.link-button:hover > span {
		display: initial;
	}
</style>
