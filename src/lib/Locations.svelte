<section>
  <div class="reviews">
    <img src="/icon-google-plus.png" alt="Google Plus" />
    <div>
      <p>Did we do a great job?</p>
      <p>Please write a Google+ review.</p>
    </div>
  </div>
  <div class="locations">
    <p>
      Serving Asheville, Buncombe County, Biltmore Forest, Black Mountain,
      Montreat, Ridgecrest, Weaverville, Woodfin, Leicester, Alexander,
      Barnardsville, Swannanoa, Fairview, Skyland, Arden, Fletcher, Candler,
      Enka
    </p>
  </div>
</section>

<style>
  section {
    max-width: 1000px;
    margin: auto;
    padding: 2rem 0;
    display: flex;
    justify-content: center;
    gap: 3rem;
  }
  div {
    display: flex;
    justify-content: flex-start;
    gap: 1rem;
  }
  div div {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    gap: 1rem;
  }
  img {
    width: 80px;
    height: 80px;
  }
  .locations,
  .reviews {
    flex: 1;
  }
  .reviews {
    align-items: center;
  }
</style>
