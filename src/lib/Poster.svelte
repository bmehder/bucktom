<script>
  import { fade } from 'svelte/transition'
</script>

<div>
  <img
    src="https://img.youtube.com/vi/Ub_XSLg-eO8/0.jpg"
    alt="Bucktom Video Poster"
    on:click
    out:fade={{ delay: 0, duration: 300 }}
  />
</div>

<style>
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>
