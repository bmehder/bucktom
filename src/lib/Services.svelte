<script>
  import { data } from '$lib/data/services'
  import Service from './Service.svelte'
</script>

<section>
  {#each data as { src, title, content }}
    <Service {src} {title} {content} />
  {/each}
</section>

<style>
  section {
    max-width: 1000px;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 1rem;
    margin: auto;
  }
</style>
