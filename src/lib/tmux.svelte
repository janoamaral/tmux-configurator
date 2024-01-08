<script context="module">
	let currentDate = new Date();

	// Format to YY-mm-dd
	let date = currentDate.getDate();
	let month = currentDate.toLocaleString('default', { month: 'long' });
	let year = currentDate.getFullYear();

	// get hour in format HH:MM
	let hour = currentDate.getHours();
	let minutes = currentDate.getMinutes();

	let dateString = `${year.toString().substring(2, 4)}-${month.substring(0, 3)}-${date
		.toString()
		.padStart(2, '0')}`;

	let timeString = `${hour.toString().padStart(2, '0')}:${minutes.toString().padStart(2, '0')}`;
</script>

<div class="tmux">
	<div class="left">[DEFAULT]&nbsp;</div>
	<div class="window">0: zsh &nbsp;1:test &nbsp;2:zsh*</div>
	<div class="right">"tmux-vm" {timeString} {dateString}</div>
</div>

<style>
	.tmux {
		font-family: 'Liga SFMono Nerd', 'FiraCode Nerd Font', monospace;
		display: flex;
		flex-direction: row;
		width: 100%;
		background: #5e931b;
		padding: 0.3rem 0;
	}

	.left {
		text-align: left;
		text-wrap: nowrap;
	}

	.window {
		text-align: left;
		text-wrap: nowrap;
	}

	.right {
		text-align: right;
		flex-grow: 1;
	}
</style>
