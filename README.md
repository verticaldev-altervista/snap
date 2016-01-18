# snap
fork of Berkeley Snap
		<script type="text/javascript" src="js/morphic.js"></script>
		<script type="text/javascript" src="js/widgets.js"></script>
		<script type="text/javascript" src="js/blocks.js"></script>
		<script type="text/javascript" src="js/threads.js"></script>
		<script type="text/javascript" src="js/objects.js"></script>
		<script type="text/javascript" src="js/gui.js"></script>
		<script type="text/javascript" src="js/paint.js"></script>
		<script type="text/javascript" src="js/lists.js"></script>
		<script type="text/javascript" src="js/byob.js"></script>
		<script type="text/javascript" src="js/xml.js"></script>
		<script type="text/javascript" src="js/store.js"></script>
		<script type="text/javascript" src="js/locale.js"></script>
		<script type="text/javascript" src="js/cloud.js"></script>
		<script type="text/javascript" src="js/sha512.js"></script>
		<script type="text/javascript">
			var world;
			window.onload = function () {
				world = new WorldMorph(document.getElementById('world'));
                world.worldCanvas.focus();
				new IDE_Morph().openIn(world);
				setInterval(loop, 1);
			};
			function loop() {
				world.doOneCycle();
			}
			document.write("<canvas id='world' tabindex='1'  />
");
		</script>
