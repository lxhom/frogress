<script>
  export let progress = 0;
</script>

<style>
#frogressbar {
  background-color: #fff;
  border-radius: 999px;
  border: 3px solid #000;
  padding: 2px;
  width: 150px;
  height: 20px;
}

#frogressbar div {
  border-radius: 999px;
  background: url(FROG.jpg);
  background-size: cover;
  height: 20px;
  background-position-x: right;
  transition: width 250ms ease-in-out;
  width: calc(var(--progress) + (150px - var(--progress)) / 150 * 20);
}
</style>

<div id="frogressbar" style="--progress: {progress ? progress : 0}%">
	<div></div>
</div>
