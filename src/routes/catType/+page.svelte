
<script>
  import { onMount } from "svelte";

  let img = [];
  const BASE_URL = `https://api.unsplash.com`;
  const API_KEY = "J8xlJ50rIrCU5MARTJ_59uX-eW75wA5TfHSnJf0ZfVU";

  onMount(() => {
    fetch(
      `${BASE_URL}/search/photos?query=cats&client_id=${API_KEY}`
    )
      .then((res) => res.json())
      .then((data) => {
        imgs.push(data.results)
      });
  });
  
</script>

{#each imgs as img}
    <img src = {img.urls.regular}/>
{/each}

<div class="Our-Cat">
  <h1>Our Cat</h1>
</div>

<div class="catCardContainer">
  <div class="slide-catCardContainer">
    <div class="card-wrapper">
      <div class="card" />
    </div>
  </div>
</div>
