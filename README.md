#Red t-shirt
<!DOCTYPE html>

<html>
 <style>
  h1 {margin: 0 40px 0 40px;
  color: red;
   }
  img {border: solid 2px;
    border-radius: 0 40px 0 40px;
  }
</style>
<head>
  <meta http-equiv="CONTENT-TYPE" content="text/html; charset=UTF-8">
  <title>Red t-shirt</title>
</head>
<body>
  <h1>Red T-shirt</h1>
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSdTaY5LvNFr-1pvAvWJ0ZSThKM87WYqM86Kw&s"><br>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>Simple Cart</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
    }

    .product {
      border: 1px solid #ddd;
      padding: 16px;
      margin-bottom: 10px;
      border-radius: 8px;
    }

    .product h3 {
      margin: 0 0 8px;
    }

    .product button {
      background-color: #28a745;
      color: white;
      border: none;
      padding: 10px 16px;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
    }

    .product button:hover {
      background-color: #218838;
    }

    #cart {
      margin-top: 30px;
      padding: 16px;
      border: 2px solid #333;
      border-radius: 10px;
      background-color: #f8f9fa;
    }
  </style>
</head>
<body>


  <div class="product">
    <h3>Large size</h3>
    <p>Price: $95</p>
    <button onclick="addToCart('Large size', 95)">Add to Cart</button>
  </div>

  <div class="product">
    <h3>Medium size</h3>
    <p>Price: $85</p>
    <button onclick="addToCart('Medium size', 85)">Add to Cart</button>
  </div>
  
  <div class="product">
    <h3>Small size</h3>
    <p>Price: $75</p>
    <button onclick="addToCart('Small size', 75)">Add to Cart</button>
  </div>
  <div id="cart">
    <h2>🛒 Cart</h2>
    <p>Items: <span id="itemCount">0</span></p>
    <p>Total: $<span id="totalPrice">0</span></p>
  </div>

  <script>
    let itemCount = 0;
    let totalPrice = 0;

    function addToCart(productName, price) {
      itemCount++;
      totalPrice += price;

      document.getElementById('itemCount').textContent = itemCount;
      document.getElementById('totalPrice').textContent = totalPrice;

      alert(productName + ' added to cart!');
    }
  </script>

</body>
</html>
