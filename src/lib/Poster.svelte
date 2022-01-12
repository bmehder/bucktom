<script>
  import { fade } from 'svelte/transition'
  import { sineInOut } from 'svelte/easing'
</script>

<div>
  <img
    src="video.jpg"
    alt="Bucktom Video Poster"
    on:click
    out:fade={{ delay: 0, duration: 300, easing: sineInOut }}
  />
</div>

<style>
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>
