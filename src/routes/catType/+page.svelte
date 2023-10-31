
<script>
  import { onMount } from "svelte";

let images = [];
const BASE_URL = "https://api.unsplash.com/search/photos";
const API_KEY = "J8xlJ50rIrCU5MARTJ_59uX-eW75wA5TfHSnJf0ZfVU";
const query = "cats";

onMount(async () => {
  try {
    const response = await fetch(`${BASE_URL}?query=${query}&client_id=${API_KEY}`);
    if (response.ok) {
      const data = await response.json();
      images = data.results;
    } else {
      console.error("Error fetching data:", response.statusText);
    }
  } catch (error) {
    console.error("Error fetching data:", error);
  }
});
</script>

<div class="Our-Cat">
<h1>Our Cat</h1>
</div>

{#each images as image}
<img src={image.urls.regular} alt="Cat" />
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
