# E-COMMERCE-PRODUCT-CARD-UI
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Product Card UI</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f0f2f5;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  .product-card {
    background: white;
    border-radius: 12px;
    width: 320px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    cursor: pointer;
  }
  .product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.2);
  }
  .product-image {
    width: 100%;
    height: 220px;
    object-fit: cover;
    transition: transform 0.3s ease;
  }
  .product-card:hover .product-image {
    transform: scale(1.05);
  }
  .content {
    padding: 20px;
  }
  .product-title {
    font-size: 1.25rem;
    color: #333;
    margin: 0 0 10px;
  }
  .product-description {
    font-size: 0.9rem;
    color: #666;
    margin-bottom: 15px;
  }
  .price-cart {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .price {
    font-size: 1.2rem;
    font-weight: bold;
    color: #007bff;
  }
  .add-to-cart {
    background-color: #28a745;
    color: white;
    border: none;
    outline: none;
    padding: 8px 15px;
    border-radius: 6px;
    cursor: pointer;
    font-size: 1rem;
    transition: background-color 0.3s ease;
  }
  .add-to-cart:hover {
    background-color: #218838;
  }
</style>
</head>
<body>

<div class="product-card" tabindex="0" aria-label="Product card">
  <img class="product-image" src="https://images.unsplash.com/photo-1600180758899-a6d63105af1c?auto=format&fit=crop&w=400&q=80" alt="Wireless Headphones" />
  <div class="content">
    <h2 class="product-title">Wireless Headphones</h2>
    <p class="product-description">Experience high-quality sound without the wires, perfect for music and calls on the go.</p>
    <div class="price-cart">
      <span class="price">$99.99</span>
      <button class="add-to-cart" onclick="addToCart()">Add to Cart</button>
    </div>
  </div>
</div>

<script>
  function addToCart() {
    alert('Item added to cart!');
  }
</script>

</body>
</html>
