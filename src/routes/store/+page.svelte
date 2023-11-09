<script>
  let product1 = "/img/catTeaser.png";
  let product2 = "/img/catToy.png";
  let imgIndex = 0;
 
  function scrollRight() {
    imgIndex++;
    if (imgIndex >= 2) {
      // Adjust this based on the number of videos
      imgIndex = 2;
    }
  }
</script>

<!-- This code represents a product section with a product category heading and a gallery of product cards. 
  Each card includes an image, product details, and price. 
  Navigation buttons allow users to browse through the product gallery. -->
<section class="product">
  <h2 class="product-category">Our Product</h2>
  <div class="gallery">
    <button class="previous-button"><i class="fa-solid fa-arrow-left" /></button
    >
    <div class="product-container">
      <div class="whole-product">
        <div class="product-card">
          <div class="product-image">
            <img src="img/catTeaser.png" class="first-product" alt="" />
          </div>
          <div class="product-info">
            <h2 class="product-brand">Cat Teaser</h2>
            <p class="product-description">
              Feather teaser wand that cats love to chase
            </p>
            <span class="price">$20</span>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image">
            <img src="img/catTeaser.png" class="first-product" alt="" />
          </div>
          <div class="product-info">
            <h2 class="product-brand">Cat Teaser</h2>
            <p class="product-description">
              Feather teaser wand that cats love to chase
            </p>
            <span class="price">$20</span>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image">
            <img src="img/catTeaser.png" class="first-product" alt="" />
          </div>
          <div class="product-info">
            <h2 class="product-brand">Cat Teaser</h2>
            <p class="product-description">
              Feather teaser wand that cats love to chase
            </p>
            <span class="price">$20</span>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image">
            <img src="img/catTeaser.png" class="first-product" alt="" />
          </div>
          <div class="product-info">
            <h2 class="product-brand">Cat Teaser</h2>
            <p class="product-description">
              Feather teaser wand that cats love to chase
            </p>
            <span class="price">$20</span>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image">
            <img src="img/catTeaser.png" class="first-product" alt="" />
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
    </div>
    <button class="next-button"><i class="fa-solid fa-arrow-left" /></button>
  </div>
</section>
