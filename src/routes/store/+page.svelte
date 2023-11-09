<script>
  let product1 = "/img/catTeaser.png";
  let product2 = "/img/catToy.png";
  let product3 = "/img/catToy2.png";
  let product4 = "/img/catToy3.png";
  let imgIndex = 0;

  // Function to scroll to the next item or image on the right.
  function scrollRight() {
    imgIndex++;
    if (imgIndex >= 1) {
      imgIndex = 1;
    }
  }

  // Function to scroll to the next item or image on the left.
  function scrollLeft() {
    imgIndex--;
    if (imgIndex < 0) {
      imgIndex = 0;
    }
  }

  // Getting image by index, return empty string for out-of-range.
  function img(index) {
    const imgArray = [product1, product2, product3, product4];

    if (index >= 0 && index < imgArray.length) {
      return imgArray[index];
    } else {
      return "";
    }
  }
</script>

<!-- This code represents a product section with a product category heading and a gallery of product cards. 
  Each card includes an image, product details, and price. 
  Navigation buttons allow users to browse through the product gallery. -->
<section class="product">
  <h2 class="product-category">Our Product</h2>
  <div class="gallery">
    <i on:click={scrollLeft} class="fa-solid fa-arrow-left previous-button" />
    <div class="product-container">
      {#each [1, 2, 3, 4] as imgProducts, i}
        {#if i >= imgIndex && i < imgIndex + 3}
          <div class="whole-product">
            <div class="product-card">
              <div class="product-image">
                <img src={img(i)} class="first-product" alt="" />
              </div>
              <div class="product-info">
                <h2 class="product-brand">Cat Teaser</h2>
                <p class="product-description">
                  Feather teaser wand that cats love to chase
                </p>
                <span class="price">$20</span>
              </div>
            </div>
          </div>
        {/if}
      {/each}
    </div>
    <i on:click={scrollRight} class="fa-solid fa-arrow-left next-button" />
  </div>
</section>
