<script>
  import { fade } from 'svelte/transition'
  import { sineInOut } from 'svelte/easing'
</script>

<iframe
  width="800"
  height="450"
  src="https://www.youtube.com/embed/Ub_XSLg-eO8"
  title="YouTube video player"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen
  in:fade={{ delay: 300, duration: 300, easing: sineInOut }}
/>
