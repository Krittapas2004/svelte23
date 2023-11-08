<!-- This code represents a product section with a product category heading and a gallery of product cards. 
  Each card includes an image, product details, and price. 
  Navigation buttons allow users to browse through the product gallery. -->

<script>
  const productContainer = [...document.querySelectorAll(".product-container")];
  const nxtButton = [...document.querySelectorAll(".next-button")];
  const preButton = [...document.querySelectorAll(".previous-button")];

  productContainer.forEach((item, i) => {
    let containerDimension =
      item.getBoundingClientRect(); /* Get the position and size of the 'item' element on the web page. */
    let containerWidth = containerDimension.width;

    nxtButton[i].addEventListener("click", () => {
      item.scrollLeft += containerWidth;
    });

    preButton[i].addEventListener("click", () => {
      item.scrollLeft -= containerWidth;
    });
  });
</script>

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
