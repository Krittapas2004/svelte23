<!-- Cat Type Page -->
<script>
  import { onMount } from "svelte";

  let allData = [];
  const BASE_URL = "https://api.unsplash.com/search/photos";
  const API_KEY = "J8xlJ50rIrCU5MARTJ_59uX-eW75wA5TfHSnJf0ZfVU";
  const query = "cats";

  /* This is for fetching the API from the unsplash website, and it will check if the API doesn't fetch */
  onMount(async () => {
    try {
      const response = await fetch(
        `${BASE_URL}?query=${query}&client_id=${API_KEY}`
      );
      if (response.ok) {
        const data = await response.json();
        allData = data.results;
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

<div class="catCard-Body">
  {#each allData as image}
    <div class="catDetail">
      <div class="gridDisplay">
        <!-- Displaying the image and the description from the API into webpage -->
        <img src={image.urls.regular} alt="Cat" />
        <p>{image.alt_description}</p>
      </div>
    </div>
  {/each}
</div>
