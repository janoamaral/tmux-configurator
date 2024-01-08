<div class="container">
	<div id="window">
		<div id="header">
			<div id="buttons">
				<div id="close"></div>
				<div id="minimize"></div>
				<div id="maximize"></div>
			</div>
			<div id="title">Tmux configurator</div>
		</div>
		<slot />
	</div>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		height: 100vh;
		justify-content: center;
		align-items: center;
	}

	#window {
		font-family: 'Liga SFMono Nerd', 'FiraCode Nerd Font', monospace !important;
		font-size: 0.9rem;
		text-rendering: optimizeLegibility;
		font-variant-ligatures: normal !important;
		display: flex;
		flex-direction: column;
		margin: 5rem;
		box-shadow: 0 20px 68px rgba(0, 0, 0, 0.55);
		border-radius: 0 0 6px 6px;
		overflow: hidden;
		width: 180ch;
	}

	#header {
		height: 40px;
		background: #1a1b26;
		border-radius: 6px 6px 0 0;
		display: flex;
		flex-direction: row;
	}

	#title {
		width: 100%;
		text-align: center;
		font-family: 'SF Pro Text', Helvetica, Arial, sans-serif;
		color: #fff;
		font-size: 14px;
		font-weight: 400;
		padding-left: 0.5rem;
		padding-top: 0.5rem;
	}

	#buttons {
		display: flex;
		height: 100%;
		padding-left: 0.5rem;
	}

	#close {
		width: 10px;
		height: 10px;
		border-radius: 50%;
		background: #ff5c57;
		margin: auto 0.2rem;
	}

	#minimize {
		width: 10px;
		height: 10px;
		border-radius: 50%;
		background: #ffbd2e;
		margin: auto 0.2rem;
	}

	#maximize {
		width: 10px;
		height: 10px;
		border-radius: 50%;
		background: #28c940;
		margin: auto 0.2rem;
	}
</style>
