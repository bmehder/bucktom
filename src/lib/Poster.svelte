<script>
  import { fade } from 'svelte/transition'
  import { sineInOut } from 'svelte/easing'
</script>

<div on:click>
  <aside>
    <svg
      class="w-6 h-6"
      fill="none"
      stroke="currentColor"
      viewBox="0 0 24 24"
      xmlns="http://www.w3.org/2000/svg"
      ><path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"
      /><path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
      /></svg
    >
    <img
      src="video.jpg"
      alt="Bucktom Video Poster"
      on:click
      out:fade={{ delay: 0, duration: 300, easing: sineInOut }}
    />
  </aside>
</div>

<style>
  div {
    position: relative;
  }
  img {
    position: relative;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  svg {
    position: absolute;
    width: 100px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 1;
    color: #b50;
  }
</style>
