<script>
  export let src = ''
  export let title = ''
  export let content = []
</script>

<article>
  <div>
    <img {src} alt={title} />
  </div>
  <h4>{title}</h4>
  <ul>
    {#each content as item}
      <li>{item}</li>
    {/each}
  </ul>
</article>

<style>
  article {
    width: 450px;
    margin: 3rem auto 0;
  }
  div {
    height: 300px;
    width: 450px;
    overflow: hidden;
    border-radius: 1rem;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  }
  img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  h4 {
    padding: 2rem 0 1rem;
    color: #b50;
  }
  ul {
    margin: 0;
    padding-left: 1rem;
  }
</style>
