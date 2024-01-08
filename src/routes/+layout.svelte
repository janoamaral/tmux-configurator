<div id="window">
	<div id="header">
		<div id="buttons">
			<div id="close"></div>
			<div id="minimize"></div>
			<div id="maximize"></div>
		</div>
		<div id="title">Tmux configuration</div>
	</div>
	<slot />
</div>

<style>
	#window {
		font-family: 'Fira Code', monospace;
		font-size: 1rem;
		display: flex;
		flex-direction: column;
		margin: 5rem;
		box-shadow: 0 20px 68px rgba(0, 0, 0, 0.55);
		border-radius: 0 0 6px 6px;
		overflow: hidden;
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

	@font-face {
		font-family: 'oxproto';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/oxproto/oxproto.woff2');
	}
	@font-face {
		font-family: 'font3270';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/font3270/font3270.ttf');
	}
	@font-face {
		font-family: 'agave';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/agave/agave.ttf');
	}
	@font-face {
		font-family: 'anka-coder';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/anka-coder/anka-coder-bold-italic.ttf');
	}
	@font-face {
		font-family: 'anka-coder';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/anka-coder/anka-coder-bold.ttf');
	}
	@font-face {
		font-family: 'anka-coder';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/anka-coder/anka-coder-italic.ttf');
	}
	@font-face {
		font-family: 'anka-coder';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/anka-coder/anka-coder.ttf');
	}
	@font-face {
		font-family: 'anonymous-pro';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/anonymous-pro/anonymous-pro-bold-italic.ttf');
	}
	@font-face {
		font-family: 'anonymous-pro';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/anonymous-pro/anonymous-pro-bold.ttf');
	}
	@font-face {
		font-family: 'anonymous-pro';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/anonymous-pro/anonymous-pro-italic.ttf');
	}
	@font-face {
		font-family: 'anonymous-pro';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/anonymous-pro/anonymous-pro.ttf');
	}
	@font-face {
		font-family: 'apl2741';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/apl2741/apl2741.ttf');
	}
	@font-face {
		font-family: 'apl385';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/apl385/apl385.ttf');
	}
	@font-face {
		font-family: 'aurulent';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/aurulent/aurulent.otf');
	}
	@font-face {
		font-family: 'average';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/average/average-bold.woff');
	}
	@font-face {
		font-family: 'average';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/average/average-bold-italic.woff');
	}
	@font-face {
		font-family: 'average';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/average/average-italic.woff');
	}
	@font-face {
		font-family: 'average';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/average/average.woff');
	}
	@font-face {
		font-family: 'azeret';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/azeret/azeret-bold-italic.ttf');
	}
	@font-face {
		font-family: 'azeret';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/azeret/azeret-bold.ttf');
	}
	@font-face {
		font-family: 'azeret';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/azeret/azeret-italic.ttf');
	}
	@font-face {
		font-family: 'azeret';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/azeret/azeret.ttf');
	}
	@font-face {
		font-family: 'bedstead';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bedstead/bedstead.otf');
	}
	@font-face {
		font-family: 'b612-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/b612-mono/b612-mono-bold-italic.ttf');
	}
	@font-face {
		font-family: 'b612-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/b612-mono/b612-mono-bold.ttf');
	}
	@font-face {
		font-family: 'b612-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/b612-mono/b612-mono-italic.ttf');
	}
	@font-face {
		font-family: 'b612-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/b612-mono/b612-mono.ttf');
	}
	@font-face {
		font-family: 'bigblue-terminal';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bigblue-terminal/bigblue-terminal.ttf');
	}
	@font-face {
		font-family: 'binchotan-sharp';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/binchotan-sharp/binchotan-sharp.ttf');
	}
	@font-face {
		font-family: 'bitstream-vera';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/bitstream-vera/bitstream-vera-bold-italic.woff');
	}
	@font-face {
		font-family: 'bitstream-vera';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bitstream-vera/bitstream-vera-bold.woff');
	}
	@font-face {
		font-family: 'bitstream-vera';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/bitstream-vera/bitstream-vera-italic.woff');
	}
	@font-face {
		font-family: 'bitstream-vera';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bitstream-vera/bitstream-vera.woff');
	}
	@font-face {
		font-family: 'borg-sans-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/borg-sans-mono/borg-sans-mono.ttf');
	}
	@font-face {
		font-family: 'bpmono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bpmono/bpmono-bold.woff');
	}
	@font-face {
		font-family: 'bpmono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/bpmono/bpmono-italic.woff');
	}
	@font-face {
		font-family: 'bpmono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bpmono/bpmono.woff');
	}
	@font-face {
		font-family: 'bront-ubuntu';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bront-ubuntu/bront-ubuntu.ttf');
	}
	@font-face {
		font-family: 'bront-dejavu';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/bront-dejavu/bront-dejavu.ttf');
	}
	@font-face {
		font-family: 'camingocode';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/camingocode/camingocode-bold-italic.woff');
	}
	@font-face {
		font-family: 'camingocode';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/camingocode/camingocode-bold.woff');
	}
	@font-face {
		font-family: 'camingocode';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/camingocode/camingocode-italic.woff');
	}
	@font-face {
		font-family: 'camingocode';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/camingocode/camingocode.woff');
	}
	@font-face {
		font-family: 'cartograph';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cartograph/cartograph-bold-italic.woff');
	}
	@font-face {
		font-family: 'cartograph';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cartograph/cartograph-bold.woff');
	}
	@font-face {
		font-family: 'cartograph';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cartograph/cartograph-italic.woff');
	}
	@font-face {
		font-family: 'cartograph';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cartograph/cartograph.woff');
	}
	@font-face {
		font-family: 'cascadia-code';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cascadia-code/cascadia-code-bold-italic.woff2');
	}
	@font-face {
		font-family: 'cascadia-code';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cascadia-code/cascadia-code-bold.woff2');
	}
	@font-face {
		font-family: 'cascadia-code';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cascadia-code/cascadia-code-italic.woff2');
	}
	@font-face {
		font-family: 'cascadia-code';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cascadia-code/cascadia-code.woff2');
	}
	@font-face {
		font-family: 'chivo';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/chivo/chivo-bold-italic.ttf');
	}
	@font-face {
		font-family: 'chivo';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/chivo/chivo-bold.ttf');
	}
	@font-face {
		font-family: 'chivo';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/chivo/chivo-italic.ttf');
	}
	@font-face {
		font-family: 'chivo';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/chivo/chivo.ttf');
	}
	@font-face {
		font-family: 'cm-unicode';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cm-unicode/cm-unicode-bold-italic.ttf');
	}
	@font-face {
		font-family: 'cm-unicode';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cm-unicode/cm-unicode-bold.ttf');
	}
	@font-face {
		font-family: 'cm-unicode';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cm-unicode/cm-unicode-italic.ttf');
	}
	@font-face {
		font-family: 'cm-unicode';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cm-unicode/cm-unicode.ttf');
	}
	@font-face {
		font-family: 'code-new-roman';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/code-new-roman/code-new-roman.otf');
	}
	@font-face {
		font-family: 'comic-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/comic-mono/comic-mono-bold.ttf');
	}
	@font-face {
		font-family: 'comic-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/comic-mono/comic-mono.ttf');
	}
	@font-face {
		font-family: 'comic-shanns';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/comic-shanns/comic-shanns.otf');
	}
	@font-face {
		font-family: 'commit-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/commit-mono/commit-mono-bold-italic.otf');
	}
	@font-face {
		font-family: 'commit-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/commit-mono/commit-mono-bold.otf');
	}
	@font-face {
		font-family: 'commit-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/commit-mono/commit-mono-italic.otf');
	}
	@font-face {
		font-family: 'commit-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/commit-mono/commit-mono.otf');
	}
	@font-face {
		font-family: 'consolamono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/consolamono/consolamono-bold.ttf');
	}
	@font-face {
		font-family: 'consolamono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/consolamono/consolamono.ttf');
	}
	@font-face {
		font-family: 'courier-prime';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime/courier-prime-bold-italic.ttf');
	}
	@font-face {
		font-family: 'courier-prime';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime/courier-prime-bold.ttf');
	}
	@font-face {
		font-family: 'courier-prime';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime/courier-prime-italic.ttf');
	}
	@font-face {
		font-family: 'courier-prime';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime/courier-prime.ttf');
	}
	@font-face {
		font-family: 'courier-prime-code';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-code/courier-prime-code-italic.ttf');
	}
	@font-face {
		font-family: 'courier-prime-code';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-code/courier-prime-code.ttf');
	}
	@font-face {
		font-family: 'courier-prime-sans';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-sans/courier-prime-sans-bold-italic.ttf');
	}
	@font-face {
		font-family: 'courier-prime-sans';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-sans/courier-prime-sans-bold.ttf');
	}
	@font-face {
		font-family: 'courier-prime-sans';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-sans/courier-prime-sans-italic.ttf');
	}
	@font-face {
		font-family: 'courier-prime-sans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/courier-prime-sans/courier-prime-sans.ttf');
	}
	@font-face {
		font-family: 'cousine';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cousine/cousine-bold-italic.woff');
	}
	@font-face {
		font-family: 'cousine';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cousine/cousine-bold.woff');
	}
	@font-face {
		font-family: 'cousine';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/cousine/cousine-italic.woff');
	}
	@font-face {
		font-family: 'cousine';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cousine/cousine.woff');
	}
	@font-face {
		font-family: 'cozette';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cozette/cozette.woff');
	}
	@font-face {
		font-family: 'cutive';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/cutive/cutive.ttf');
	}
	@font-face {
		font-family: 'd2coding';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/d2coding/d2coding.ttf');
	}
	@font-face {
		font-family: 'd2coding';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/d2coding/d2coding-bold.ttf');
	}
	@font-face {
		font-family: 'daddytimemono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/daddytimemono/daddytimemono.ttf');
	}
	@font-face {
		font-family: 'dejavu';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/dejavu/dejavu-bold-italic.woff');
	}
	@font-face {
		font-family: 'dejavu';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/dejavu/dejavu-bold.woff');
	}
	@font-face {
		font-family: 'dejavu';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/dejavu/dejavu-italic.woff');
	}
	@font-face {
		font-family: 'dejavu';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/dejavu/dejavu.woff');
	}
	@font-face {
		font-family: 'dm-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/dm-mono/dm-mono-italic.woff');
	}
	@font-face {
		font-family: 'dm-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/dm-mono/dm-mono-regular.woff');
	}
	@font-face {
		font-family: 'drafting';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/drafting/drafting-bold-italic.woff2');
	}
	@font-face {
		font-family: 'drafting';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/drafting/drafting-bold.woff2');
	}
	@font-face {
		font-family: 'drafting';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/drafting/drafting-italic.woff2');
	}
	@font-face {
		font-family: 'drafting';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/drafting/drafting.woff2');
	}
	@font-face {
		font-family: 'droid-sans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/droid-sans/droid-sans.woff');
	}
	@font-face {
		font-family: 'edlo';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/edlo/edlo.ttf');
	}
	@font-face {
		font-family: 'effects-eighty';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/effects-eighty/effects-eighty-bold-italic.otf');
	}
	@font-face {
		font-family: 'effects-eighty';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/effects-eighty/effects-eighty-bold.otf');
	}
	@font-face {
		font-family: 'effects-eighty';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/effects-eighty/effects-eighty-italic.otf');
	}
	@font-face {
		font-family: 'effects-eighty';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/effects-eighty/effects-eighty.otf');
	}
	@font-face {
		font-family: 'ellograph';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ellograph/ellograph-bold-italic.woff');
	}
	@font-face {
		font-family: 'ellograph';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ellograph/ellograph-bold.woff');
	}
	@font-face {
		font-family: 'ellograph';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ellograph/ellograph-italic.woff');
	}
	@font-face {
		font-family: 'ellograph';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ellograph/ellograph.woff');
	}
	@font-face {
		font-family: 'envy-code-b';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/envy-code-b/envy-code-b.ttf');
	}
	@font-face {
		font-family: 'envy-code-r';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/envy-code-r/envy-code-r-bold.woff');
	}
	@font-face {
		font-family: 'envy-code-r';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/envy-code-r/envy-code-r-italic.woff');
	}
	@font-face {
		font-family: 'envy-code-r';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/envy-code-r/envy-code-r.woff');
	}
	@font-face {
		font-family: 'fairfax';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax/fairfax-bold.ttf');
	}
	@font-face {
		font-family: 'fairfax';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax/fairfax-italic.ttf');
	}
	@font-face {
		font-family: 'fairfax';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax/fairfax.ttf');
	}
	@font-face {
		font-family: 'fairfax-hd';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax-hd/fairfax-hd.ttf');
	}
	@font-face {
		font-family: 'fairfax-hd-hax';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax-hd-hax/fairfax-hd-hax.ttf');
	}
	@font-face {
		font-family: 'fairfax-serif';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fairfax-serif/fairfax-serif.ttf');
	}
	@font-face {
		font-family: 'fantasque-sans';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/fantasque-sans/fantasque-sans-bold-italic.woff');
	}
	@font-face {
		font-family: 'fantasque-sans';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fantasque-sans/fantasque-sans-bold.woff');
	}
	@font-face {
		font-family: 'fantasque-sans';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/fantasque-sans/fantasque-sans-italic.woff');
	}
	@font-face {
		font-family: 'fantasque-sans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fantasque-sans/fantasque-sans.woff');
	}
	@font-face {
		font-family: 'fifteen';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fifteen/fifteen.ttf');
	}
	@font-face {
		font-family: 'fira';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fira/fira-bold.woff');
	}
	@font-face {
		font-family: 'fira';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fira/fira.woff');
	}
	@font-face {
		font-family: 'firacode';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/firacode/firacode-bold.woff2');
	}
	@font-face {
		font-family: 'firacode';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/firacode/firacode.woff2');
	}
	@font-face {
		font-family: 'fixedsys';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fixedsys/fixedsys.woff');
	}
	@font-face {
		font-family: 'fixedsys-ligatures';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fixedsys-ligatures/fixedsys-ligatures.ttf');
	}
	@font-face {
		font-family: 'fragment-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/fragment-mono/fragment-mono-italic.woff2');
	}
	@font-face {
		font-family: 'fragment-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/fragment-mono/fragment-mono.woff2');
	}
	@font-face {
		font-family: 'geist';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/geist/geist-bold.woff2');
	}
	@font-face {
		font-family: 'geist';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/geist/geist.woff2');
	}
	@font-face {
		font-family: 'generic';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/generic/generic.otf');
	}
	@font-face {
		font-family: 'gintronic';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/gintronic/gintronic-italic.woff2');
	}
	@font-face {
		font-family: 'gintronic';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/gintronic/gintronic.woff2');
	}
	@font-face {
		font-family: 'gnu-freefont';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/gnu-freefont/gnu-freefont-bold-italic.woff');
	}
	@font-face {
		font-family: 'gnu-freefont';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/gnu-freefont/gnu-freefont-bold.woff');
	}
	@font-face {
		font-family: 'gnu-freefont';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/gnu-freefont/gnu-freefont-italic.woff');
	}
	@font-face {
		font-family: 'gnu-freefont';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/gnu-freefont/gnu-freefont.woff');
	}
	@font-face {
		font-family: 'go-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/go-mono/go-mono-bold-italic.ttf');
	}
	@font-face {
		font-family: 'go-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/go-mono/go-mono-bold.ttf');
	}
	@font-face {
		font-family: 'go-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/go-mono/go-mono-italic.ttf');
	}
	@font-face {
		font-family: 'go-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/go-mono/go-mono.ttf');
	}
	@font-face {
		font-family: 'gohufont-11';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/gohufont-11/gohufont-11.ttf');
	}
	@font-face {
		font-family: 'gohufont-14';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/gohufont-14/gohufont-14.ttf');
	}
	@font-face {
		font-family: 'hack';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hack/hack-bold-italic.woff');
	}
	@font-face {
		font-family: 'hack';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hack/hack-bold.woff');
	}
	@font-face {
		font-family: 'hack';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hack/hack-italic.woff');
	}
	@font-face {
		font-family: 'hack';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hack/hack.woff');
	}
	@font-face {
		font-family: 'hasklig';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hasklig/hasklig-bold-italic.otf');
	}
	@font-face {
		font-family: 'hasklig';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hasklig/hasklig-bold.otf');
	}
	@font-face {
		font-family: 'hasklig';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hasklig/hasklig-italic.otf');
	}
	@font-face {
		font-family: 'hasklig';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hasklig/hasklig.otf');
	}
	@font-face {
		font-family: 'hermit';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hermit/hermit-bold-italic.woff2');
	}
	@font-face {
		font-family: 'hermit';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hermit/hermit-bold.woff2');
	}
	@font-face {
		font-family: 'hermit';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/hermit/hermit-italic.woff2');
	}
	@font-face {
		font-family: 'hermit';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/hermit/hermit.woff2');
	}
	@font-face {
		font-family: 'heterodox-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/heterodox-mono/heterodox-mono-bold.otf');
	}
	@font-face {
		font-family: 'heterodox-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/heterodox-mono/heterodox-mono.otf');
	}
	@font-face {
		font-family: 'ia-writer-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ia-writer-mono/ia-writer-mono.woff');
	}
	@font-face {
		font-family: 'ia-writer-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ia-writer-mono/ia-writer-mono-italic.woff');
	}
	@font-face {
		font-family: 'ia-writer-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ia-writer-mono/ia-writer-mono-bold.woff');
	}
	@font-face {
		font-family: 'ia-writer-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ia-writer-mono/ia-writer-mono-bold-italic.woff');
	}
	@font-face {
		font-family: 'ibm-vga';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ibm-vga/ibm-vga.woff');
	}
	@font-face {
		font-family: 'intel-one-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/intel-one-mono/intel-one-mono.woff2');
	}
	@font-face {
		font-family: 'intel-one-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/intel-one-mono/intel-one-mono-italic.woff2');
	}
	@font-face {
		font-family: 'intel-one-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/intel-one-mono/intel-one-mono-bold.woff2');
	}
	@font-face {
		font-family: 'intel-one-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/intel-one-mono/intel-one-mono-bolditalic.woff2');
	}
	@font-face {
		font-family: 'iosevka';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/iosevka/iosevka.woff2');
	}
	@font-face {
		font-family: 'iosevka';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/iosevka/iosevka-italic.woff2');
	}
	@font-face {
		font-family: 'iosevka';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/iosevka/iosevka-bold.woff2');
	}
	@font-face {
		font-family: 'iosevka';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/iosevka/iosevka-bold-italic.woff2');
	}
	@font-face {
		font-family: 'inconsolata';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata/inconsolata-bold.ttf');
	}
	@font-face {
		font-family: 'inconsolata';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata/inconsolata.ttf');
	}
	@font-face {
		font-family: 'inconsolata-otf';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata-otf/inconsolata-otf.otf');
	}
	@font-face {
		font-family: 'inconsolata-go';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata-go/inconsolata-go-bold.ttf');
	}
	@font-face {
		font-family: 'inconsolata-go';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata-go/inconsolata-go.ttf');
	}
	@font-face {
		font-family: 'inconsolata-g';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/inconsolata-g/inconsolata-g.otf');
	}
	@font-face {
		font-family: 'jetbrainsmono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/jetbrainsmono/jetbrainsmono.woff');
	}
	@font-face {
		font-family: 'jetbrainsmono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/jetbrainsmono/jetbrainsmono-italic.woff');
	}
	@font-face {
		font-family: 'jetbrainsmono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/jetbrainsmono/jetbrainsmono-bold.woff');
	}
	@font-face {
		font-family: 'jetbrainsmono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/jetbrainsmono/jetbrainsmono-bold-italic.woff');
	}
	@font-face {
		font-family: 'julia-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/julia-mono/julia-mono-bold.ttf');
	}
	@font-face {
		font-family: 'julia-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/julia-mono/julia-mono.ttf');
	}
	@font-face {
		font-family: 'latin-modern';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/latin-modern/latin-modern-italic.woff');
	}
	@font-face {
		font-family: 'latin-modern';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/latin-modern/latin-modern.woff');
	}
	@font-face {
		font-family: 'league';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/league/league-bold.woff');
	}
	@font-face {
		font-family: 'league';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/league/league.woff');
	}
	@font-face {
		font-family: 'lekton';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/lekton/lekton-bold.ttf');
	}
	@font-face {
		font-family: 'lekton';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/lekton/lekton-italic.ttf');
	}
	@font-face {
		font-family: 'lekton';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/lekton/lekton.ttf');
	}
	@font-face {
		font-family: 'liberation';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/liberation/liberation-bold-italic.woff');
	}
	@font-face {
		font-family: 'liberation';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/liberation/liberation-bold.woff');
	}
	@font-face {
		font-family: 'liberation';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/liberation/liberation-italic.woff');
	}
	@font-face {
		font-family: 'liberation';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/liberation/liberation.woff');
	}
	@font-face {
		font-family: 'lilex';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/lilex/lilex-regular.woff');
	}
	@font-face {
		font-family: 'lilex';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/lilex/lilex-bold.woff');
	}
	@font-face {
		font-family: 'lotion';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/lotion/lotion.woff2');
	}
	@font-face {
		font-family: 'luculent';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/luculent/luculent-bold-italic.woff');
	}
	@font-face {
		font-family: 'luculent';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/luculent/luculent-bold.woff');
	}
	@font-face {
		font-family: 'luculent';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/luculent/luculent-italic.woff');
	}
	@font-face {
		font-family: 'luculent';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/luculent/luculent.woff');
	}
	@font-face {
		font-family: 'luxi';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/luxi/luxi-bold-italic.woff');
	}
	@font-face {
		font-family: 'luxi';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/luxi/luxi-bold.woff');
	}
	@font-face {
		font-family: 'luxi';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/luxi/luxi-italic.woff');
	}
	@font-face {
		font-family: 'luxi';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/luxi/luxi.woff');
	}
	@font-face {
		font-family: 'maple';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/maple/maple-bold-italic.woff2');
	}
	@font-face {
		font-family: 'maple';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/maple/maple-bold.woff2');
	}
	@font-face {
		font-family: 'maple';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/maple/maple-italic.woff2');
	}
	@font-face {
		font-family: 'maple';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/maple/maple.woff2');
	}
	@font-face {
		font-family: 'martian-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/martian-mono/martian-mono-bold.woff2');
	}
	@font-face {
		font-family: 'martian-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/martian-mono/martian-mono.woff2');
	}
	@font-face {
		font-family: 'mensch';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/mensch/mensch.ttf');
	}
	@font-face {
		font-family: 'meslo';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/meslo/meslo-bold-italic.woff');
	}
	@font-face {
		font-family: 'meslo';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/meslo/meslo-bold.woff');
	}
	@font-face {
		font-family: 'meslo';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/meslo/meslo-italic.woff');
	}
	@font-face {
		font-family: 'meslo';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/meslo/meslo.woff');
	}
	@font-face {
		font-family: 'monaspace-argon';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-argon/monaspace-argon-bold-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-argon';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-argon/monaspace-argon-bold.woff');
	}
	@font-face {
		font-family: 'monaspace-argon';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-argon/monaspace-argon-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-argon';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-argon/monaspace-argon.woff');
	}
	@font-face {
		font-family: 'monaspace-krypton';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-krypton/monaspace-krypton-bold-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-krypton';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-krypton/monaspace-krypton-bold.woff');
	}
	@font-face {
		font-family: 'monaspace-krypton';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-krypton/monaspace-krypton-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-krypton';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-krypton/monaspace-krypton.woff');
	}
	@font-face {
		font-family: 'monaspace-neon';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-neon/monaspace-neon-bold-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-neon';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-neon/monaspace-neon-bold.woff');
	}
	@font-face {
		font-family: 'monaspace-neon';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-neon/monaspace-neon-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-neon';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-neon/monaspace-neon.woff');
	}
	@font-face {
		font-family: 'monaspace-radon';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-radon/monaspace-radon-bold-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-radon';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-radon/monaspace-radon-bold.woff');
	}
	@font-face {
		font-family: 'monaspace-radon';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-radon/monaspace-radon-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-radon';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-radon/monaspace-radon.woff');
	}
	@font-face {
		font-family: 'monaspace-xenon';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-xenon/monaspace-xenon-bold-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-xenon';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-xenon/monaspace-xenon-bold.woff');
	}
	@font-face {
		font-family: 'monaspace-xenon';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-xenon/monaspace-xenon-italic.woff');
	}
	@font-face {
		font-family: 'monaspace-xenon';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monaspace-xenon/monaspace-xenon.woff');
	}
	@font-face {
		font-family: 'monocraft';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monocraft/monocraft.ttf');
	}
	@font-face {
		font-family: 'monoflow';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monoflow/monoflow-italic.woff2');
	}
	@font-face {
		font-family: 'monoflow';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monoflow/monoflow.woff2');
	}
	@font-face {
		font-family: 'monofoki';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monofoki/monofoki-bold-italic.otf');
	}
	@font-face {
		font-family: 'monofoki';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monofoki/monofoki-bold.otf');
	}
	@font-face {
		font-family: 'monofoki';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monofoki/monofoki-italic.otf');
	}
	@font-face {
		font-family: 'monofoki';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monofoki/monofoki.otf');
	}
	@font-face {
		font-family: 'monofur';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monofur/monofur-italic.woff');
	}
	@font-face {
		font-family: 'monofur';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monofur/monofur.woff');
	}
	@font-face {
		font-family: 'monoid';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monoid/monoid-bold.ttf');
	}
	@font-face {
		font-family: 'monoid';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/monoid/monoid-italic.ttf');
	}
	@font-face {
		font-family: 'monoid';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/monoid/monoid.ttf');
	}
	@font-face {
		font-family: 'mononoki';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/mononoki/mononoki-bold-italic.woff');
	}
	@font-face {
		font-family: 'mononoki';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/mononoki/mononoki-bold.woff');
	}
	@font-face {
		font-family: 'mononoki';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/mononoki/mononoki-italic.woff');
	}
	@font-face {
		font-family: 'mononoki';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/mononoki/mononoki.woff');
	}
	@font-face {
		font-family: 'mplus';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/mplus/mplus-bold.ttf');
	}
	@font-face {
		font-family: 'mplus';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/mplus/mplus.ttf');
	}
	@font-face {
		font-family: 'nanum-gothic-coding';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/nanum-gothic-coding/nanum-gothic-coding-bold.ttf');
	}
	@font-face {
		font-family: 'nanum-gothic-coding';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/nanum-gothic-coding/nanum-gothic-coding.ttf');
	}
	@font-face {
		font-family: 'notcouriersans';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/notcouriersans/notcouriersans-bold.woff');
	}
	@font-face {
		font-family: 'notcouriersans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/notcouriersans/notcouriersans.woff');
	}
	@font-face {
		font-family: 'noto';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/noto/noto.ttf');
	}
	@font-face {
		font-family: 'nova';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/nova/nova.ttf');
	}
	@font-face {
		font-family: 'nova';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/nova/nova.ttf');
	}
	@font-face {
		font-family: 'office-code-pro';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/office-code-pro/office-code-pro-bold-italic.woff');
	}
	@font-face {
		font-family: 'office-code-pro';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/office-code-pro/office-code-pro-bold.woff');
	}
	@font-face {
		font-family: 'office-code-pro';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/office-code-pro/office-code-pro-italic.woff');
	}
	@font-face {
		font-family: 'office-code-pro';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/office-code-pro/office-code-pro.woff');
	}
	@font-face {
		font-family: 'opendyslexic';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/opendyslexic/opendyslexic.otf');
	}
	@font-face {
		font-family: 'overpass';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/overpass/overpass.woff');
	}
	@font-face {
		font-family: 'overpass';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/overpass/overpass.woff');
	}
	@font-face {
		font-family: 'oxygen';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/oxygen/oxygen.otf');
	}
	@font-face {
		font-family: 'plex-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/plex-mono/plex-mono-semibold-italic.woff');
	}
	@font-face {
		font-family: 'plex-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/plex-mono/plex-mono-semibold.woff');
	}
	@font-face {
		font-family: 'plex-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/plex-mono/plex-mono-italic.woff');
	}
	@font-face {
		font-family: 'plex-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/plex-mono/plex-mono.woff');
	}
	@font-face {
		font-family: 'press-start-2p';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/press-start-2p/press-start-2p.ttf');
	}
	@font-face {
		font-family: 'profont';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/profont/profont.woff');
	}
	@font-face {
		font-family: 'proggy-clean';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/proggy-clean/proggy-clean.woff');
	}
	@font-face {
		font-family: 'proggy-vector';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/proggy-vector/proggy-vector.woff');
	}
	@font-face {
		font-family: 'pt';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/pt/pt.woff');
	}
	@font-face {
		font-family: 'pt';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/pt/pt-bold.woff');
	}
	@font-face {
		font-family: 'quinze';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/quinze/quinze.ttf');
	}
	@font-face {
		font-family: 'recursive-mono-linear';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/recursive-mono-linear/recursive-mono-linear-bold-italic.ttf');
	}
	@font-face {
		font-family: 'recursive-mono-linear';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/recursive-mono-linear/recursive-mono-linear-bold.ttf');
	}
	@font-face {
		font-family: 'recursive-mono-linear';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/recursive-mono-linear/recursive-mono-linear-italic.ttf');
	}
	@font-face {
		font-family: 'recursive-mono-linear';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/recursive-mono-linear/recursive-mono-linear.ttf');
	}
	@font-face {
		font-family: 'reddit-sans';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/reddit-sans/reddit-sans-bold.woff2');
	}
	@font-face {
		font-family: 'reddit-sans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/reddit-sans/reddit-sans.woff2');
	}
	@font-face {
		font-family: 'redhat';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/redhat/redhat-bold-italic.woff2');
	}
	@font-face {
		font-family: 'redhat';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/redhat/redhat-bold.woff2');
	}
	@font-face {
		font-family: 'redhat';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/redhat/redhat-italic.woff2');
	}
	@font-face {
		font-family: 'redhat';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/redhat/redhat.woff2');
	}
	@font-face {
		font-family: 'roboto';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/roboto/roboto-bold-italic.woff');
	}
	@font-face {
		font-family: 'roboto';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/roboto/roboto-bold.woff');
	}
	@font-face {
		font-family: 'roboto';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/roboto/roboto-italic.woff');
	}
	@font-face {
		font-family: 'roboto';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/roboto/roboto.woff');
	}
	@font-face {
		font-family: 'sax';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sax/sax.woff');
	}
	@font-face {
		font-family: 'scientifica';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/scientifica/scientifica.ttf');
	}
	@font-face {
		font-family: 'scientifica';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/scientifica/scientifica-bold.ttf');
	}
	@font-face {
		font-family: 'scientifica';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/scientifica/scientifica-italic.ttf');
	}
	@font-face {
		font-family: 'serious-sans';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/serious-sans/serious-sans-bold-italic.ttf');
	}
	@font-face {
		font-family: 'serious-sans';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/serious-sans/serious-sans-bold.ttf');
	}
	@font-face {
		font-family: 'serious-sans';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/serious-sans/serious-sans-italic.ttf');
	}
	@font-face {
		font-family: 'serious-sans';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/serious-sans/serious-sans.ttf');
	}
	@font-face {
		font-family: 'share-tech';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/share-tech/share-tech.ttf');
	}
	@font-face {
		font-family: 'sk-modernist';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sk-modernist/sk-modernist.woff');
	}
	@font-face {
		font-family: 'sono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sono/sono-bold.woff2');
	}
	@font-face {
		font-family: 'sono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sono/sono.woff2');
	}
	@font-face {
		font-family: 'source-code-pro';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/source-code-pro/source-code-pro-bold.woff');
	}
	@font-face {
		font-family: 'source-code-pro';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/source-code-pro/source-code-pro.woff');
	}
	@font-face {
		font-family: 'source-code-pro';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/source-code-pro/source-code-pro-bold-italic.woff');
	}
	@font-face {
		font-family: 'source-code-pro';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/source-code-pro/source-code-pro-italic.woff');
	}
	@font-face {
		font-family: 'space';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/space/space-bold.ttf');
	}
	@font-face {
		font-family: 'space';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/space/space.ttf');
	}
	@font-face {
		font-family: 'space';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/space/space-bold-italic.ttf');
	}
	@font-face {
		font-family: 'space';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/space/space-italic.ttf');
	}
	@font-face {
		font-family: 'spleen';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/spleen/spleen.otf');
	}
	@font-face {
		font-family: 'sudo';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/sudo/sudo-bold-italic.ttf');
	}
	@font-face {
		font-family: 'sudo';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sudo/sudo-bold.ttf');
	}
	@font-face {
		font-family: 'sudo';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/sudo/sudo-italic.ttf');
	}
	@font-face {
		font-family: 'sudo';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sudo/sudo.ttf');
	}
	@font-face {
		font-family: 'sometype-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/sometype-mono/sometype-mono-bold-italic.woff');
	}
	@font-face {
		font-family: 'sometype-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sometype-mono/sometype-mono-bold.woff');
	}
	@font-face {
		font-family: 'sometype-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/sometype-mono/sometype-mono-regular-italic.woff');
	}
	@font-face {
		font-family: 'sometype-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/sometype-mono/sometype-mono-regular.woff');
	}
	@font-face {
		font-family: 'tex-gyre-cursor';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/tex-gyre-cursor/tex-gyre-cursor-bold-italic.woff');
	}
	@font-face {
		font-family: 'tex-gyre-cursor';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/tex-gyre-cursor/tex-gyre-cursor-bold.woff');
	}
	@font-face {
		font-family: 'tex-gyre-cursor';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/tex-gyre-cursor/tex-gyre-cursor-italic.woff');
	}
	@font-face {
		font-family: 'tex-gyre-cursor';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/tex-gyre-cursor/tex-gyre-cursor.woff');
	}
	@font-face {
		font-family: 'terminus';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/terminus/terminus-bold-italic.ttf');
	}
	@font-face {
		font-family: 'terminus';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/terminus/terminus-bold.ttf');
	}
	@font-face {
		font-family: 'terminus';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/terminus/terminus-italic.ttf');
	}
	@font-face {
		font-family: 'terminus';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/terminus/terminus.ttf');
	}
	@font-face {
		font-family: 'twilio-sans-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/twilio-sans-mono/twilio-sans-mono-bold-italic.woff2');
	}
	@font-face {
		font-family: 'twilio-sans-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/twilio-sans-mono/twilio-sans-mono-bold.woff2');
	}
	@font-face {
		font-family: 'twilio-sans-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/twilio-sans-mono/twilio-sans-mono-italic.woff2');
	}
	@font-face {
		font-family: 'twilio-sans-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/twilio-sans-mono/twilio-sans-mono.woff2');
	}
	@font-face {
		font-family: 'ubuntu';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ubuntu/ubuntu-bold-italic.ttf');
	}
	@font-face {
		font-family: 'ubuntu';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ubuntu/ubuntu-bold.ttf');
	}
	@font-face {
		font-family: 'ubuntu';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/ubuntu/ubuntu-italic.ttf');
	}
	@font-face {
		font-family: 'ubuntu';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/ubuntu/ubuntu.ttf');
	}
	@font-face {
		font-family: 'unifont';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/unifont/unifont.woff');
	}
	@font-face {
		font-family: 'unifontex';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/unifontex/unifontex.ttf');
	}
	@font-face {
		font-family: 'verily';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/verily/verily.woff');
	}
	@font-face {
		font-family: 'victor-mono';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/victor-mono/victor-mono.woff');
	}
	@font-face {
		font-family: 'victor-mono';
		font-weight: normal;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/victor-mono/victor-mono-italic.woff');
	}
	@font-face {
		font-family: 'victor-mono';
		font-weight: bold;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/victor-mono/victor-mono-bold.woff');
	}
	@font-face {
		font-family: 'victor-mono';
		font-weight: bold;
		font-style: italic;
		src: url('https://www.programmingfonts.org/fonts/resources/victor-mono/victor-mono-bold-italic.woff');
	}
	@font-face {
		font-family: 'vt323';
		font-weight: normal;
		font-style: normal;
		src: url('https://www.programmingfonts.org/fonts/resources/vt323/vt323.ttf');
	}
</style>
