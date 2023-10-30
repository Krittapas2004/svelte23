<script>
  import { onMount } from "svelte";

  let imgs = [];
  const BASE_URL = `https://api.unsplash.com`;
  onMount(() => {
    fetch(
      `${BASE_URL}/search/photos?query=cats&client_id=J8xlJ50rIrCU5MARTJ_59uX-eW75wA5TfHSnJf0ZfVU`
    )
      .then((res) => res.json())
      .then((data) => {
        imgs = data.results;
      });
  });
</script>

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
