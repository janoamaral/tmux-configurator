<script>
	import Tmux from '../lib/tmux.svelte';
</script>

<div class="terminal">
	<pre>⚡ ~ ls -la</pre>
</div>
<Tmux />

<style>
	.terminal {
		height: 80vh;
		color: #c0caf5;
		background-color: #1a1b26;
		padding: 1rem;
	}
</style>
