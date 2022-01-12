<script>
  import Video from '$lib/Video.svelte'
  import Poster from '$lib/Poster.svelte'

  let component = Poster
</script>

<section>
  <div>
    <h2>BuckTom Services, LLC</h2>
    <h3>Serving Asheville and Buncombe County</h3>
    <p>
      We are a complete tree service, commercial residential lawn care, and
      landscaping company, specializing in tree removal, tree cutting, tree
      pruning services, and total lawn care in Asheville and Buncombe County.
    </p>
    <aside>
      <svelte:component this={component} on:click={() => (component = Video)} />
    </aside>
  </div>
</section>

<style>
  section {
    color: #ffd;
    padding: 4em;
    border-width: 9px 0;
    border-style: solid;
    border-color: #001100;
    background: url('/bg.jpg') no-repeat center center/cover;
    overflow: hidden;
  }
  div {
    max-width: 1000px;
    margin: auto;
  }
  h2 {
    padding: 0.5em 0;
    text-align: center;
    font-size: 3em;
  }
  h3 {
    padding: 0.5em 0 1.5em;
    text-align: center;
    font-size: 1.5em;
    font-weight: normal;
  }
  p {
    width: 80%;
    margin: auto;
    font-size: 1.1rem;
    line-height: 1.5em;
  }
  aside {
    width: 800px;
    height: auto;
    display: block;
    margin: 2rem auto;
  }
</style>
