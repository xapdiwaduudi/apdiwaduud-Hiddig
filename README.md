<html>
 <head>  
 </head> 
 <body> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Doonka Delivery - Dark &amp; Light Mode</title> 
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      transition: background-color 0.3s, color 0.3s;
    }

    /* Light Mode */
    body.light-mode {
      background-color: #fefefe;
      color: #000;
    }

    /* Dark Mode */
    body.dark-mode {
      background-color: #121212;
      color: #fff;
    }

    .container {
      max-width: 800px;
      margin: auto;
      padding: 20px;
    }

    .toggle-btn {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 20px;
      background-color: #444;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .toggle-btn:hover {
      background-color: #222;
    }

    h1 {
      text-align: center;
    }

    .food-card {
      background-color: inherit;
      padding: 15px;
      border: 1px solid #888;
      border-radius: 10px;
      margin-bottom: 15px;
    }

    .dark-mode .food-card {
      border-color: #555;
    }
  </style> 
  <!-- Dark/Light Mode Button --> 
  <button class="toggle-btn" onclick="toggleMode()">Dark Mode</button> 
  <script>
    function toggleMode() {
      document.body.classList.toggle('dark-mode');
      document.body.classList.toggle('light-mode');
      const btn = document.querySelector('.toggle-btn');
      btn.textContent = document.body.classList.contains('dark-mode') ? 'Light Mode' : 'Dark Mode';
    }
  </script> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Doonka Delivery</title> 
  <style>
    body {
      font-family: sans-serif;
      margin: 0;
      background: #fff;
    }

    header {
      background-color: #a40000;
      color: white;
      padding: 15px;
      text-align: center;
      font-size: 20px;
    }

    main {
      padding: 20px;
    }

    h2 {
      font-size: 24px;
      margin-bottom: 10px;
    }

    #search {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      margin-bottom: 20px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 15px;
    }

    .card {
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 0 5px rgba(0,0,0,0.1);
      text-align: center;
      background: #f9f9f9;
      padding-bottom: 10px;
    }

    .card img {
      width: 100%;
      height: 140px;
      object-fit: cover;
    }

    .card h3 {
      margin: 10px 0 0 0;
      font-size: 18px;
    }

    .card p {
      color: gray;
      margin-bottom: 10px;
    }

    button {
      margin-top: 10px;
      padding: 10px 20px;
      background-color: #a40000;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    button:hover {
      background-color: #870000;
    }

    footer nav {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      background: #fff;
      display: flex;
      justify-content: space-around;
      border-top: 1px solid #ccc;
      padding: 10px 0;
    }

    footer nav a {
      text-decoration: none;
      color: #a40000;
      font-weight: bold;
      font-size: 14px;
    }

    .page {
      display: none;
    }

    .active {
      display: block;
    }
  </style> 
  <header> 
   <h1>Doonka Delivery</h1> 
  </header> 
  <main id="homePage"> 
   <h2>Halkan ka raadi cuntada ama cabitaanka aad rabto</h2> 
   <input type="text" id="search" placeholder="Raadi..."> 
   <div class="grid"> 
    <!-- Cuntada --> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTr6qzPSxdAVyfxybsoMeDQRbqstirUo1rIxRNDSskoRQ&amp;s"> 
     <h3>Burger</h3> 
     <p>3.99$ dollar</p> 
     <button onclick="openOrder('Burger', 3.99, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTr6qzPSxdAVyfxybsoMeDQRbqstirUo1rIxRNDSskoRQ&amp;s')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSy05BrVSFN4wWKGl7UnjnCa2FGw_in4Qfo6AHotZ9lelf2HXnNeJfVzRU&amp;s=10"> 
     <h3>Pizza</h3> 
     <p>7.99$ dollar</p> 
     <button onclick="openOrder('Pizza', 7.99, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSy05BrVSFN4wWKGl7UnjnCa2FGw_in4Qfo6AHotZ9lelf2HXnNeJfVzRU&amp;s=10')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTsH1EXFzklT_1TKmdDlCYhJ5yeOsK7qjWw_g&amp;usqp=CAU"> 
     <h3>chicken chips</h3> 
     <p>1.99$ dollar</p> 
     <button onclick="openOrder('chicken chips', 1.99, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTsH1EXFzklT_1TKmdDlCYhJ5yeOsK7qjWw_g&amp;usqp=CAU')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTMUzMgrXH7ORYyPWwLIILsnq2ih0mmjE3sAQ&amp;usqp=CAU"> 
     <h3>Shuwaarma</h3> 
     <p>3.99$ dollar</p> 
     <button onclick="openOrder('Shuwaarma', 3.99, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTMUzMgrXH7ORYyPWwLIILsnq2ih0mmjE3sAQ&amp;usqp=CAU')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAhEqoZt10aUl-nGPOME6jztgDKtTFHiND57bxH_2NNQ&amp;s"> 
     <h3>Bariis iyo Chicken</h3> 
     <p>3.99$ dollar</p> 
     <button onclick="openOrder('Bariis iyo Chicken', 3.99, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAhEqoZt10aUl-nGPOME6jztgDKtTFHiND57bxH_2NNQ&amp;s')">Dalbo Hadda</button> 
    </div> 
    <!-- Cabitaanno --> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSSSJl9w5CkqQbHSxH56l8ksjIrSr2wDtsBjYx_rsQjta0O2ZgfxAIvAB8&amp;s=10"> 
     <h3>Watermelon Juice</h3> 
     <p>2.50$ dollar</p> 
     <button onclick="openOrder('Watermelon Juice', 2.50, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSSSJl9w5CkqQbHSxH56l8ksjIrSr2wDtsBjYx_rsQjta0O2ZgfxAIvAB8&amp;s=10')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQRmBQ7hsBm1St5ugA76cnFRBfgcCTJxiESD58Q4kcazUAYw5r_igtbXUTV&amp;s=10"> 
     <h3>blue ocean juice </h3> 
     <p>2.50$ dollar</p> 
     <button onclick="openOrder('blue ocean Juice', 2.50, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQRmBQ7hsBm1St5ugA76cnFRBfgcCTJxiESD58Q4kcazUAYw5r_igtbXUTV&amp;s=10')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://californiaavocado.com/wp-content/uploads/2020/08/Avocado-Milkshake-3-1.jpg" "> 
     <h3>avocado juice </h3> 
     <p>2.50$ dollar</p> 
     <button onclick="openOrder('avocado Juice', 2.50, 'https://californiaavocado.com/wp-content/uploads/2020/08/Avocado-Milkshake-3-1.jpg')">Dalbo Hadda</button> 
    </div> 
    <div class="card"> 
     <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQci2LuLjao5Gs6CTbqr3evOEtwDpK6RKocFQ&amp;s"> 
     <h3>Mango Juice</h3> 
     <p>2.50$ dollar</p> 
     <button onclick="openOrder('Mango Juice', 2.50, 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQci2LuLjao5Gs6CTbqr3evOEtwDpK6RKocFQ&amp;s')">Dalbo Hadda</button> 
    </div> 
   </div> 
  </main> 
  <div id="orderPage" class="page" style="text-align: center;"> 
   <h2 id="orderTitle"></h2> 
   <img id="orderImage" src="" style="width: 200px; border-radius: 10px;"> 
   <p>Qiimaha: <strong id="itemPriceText"></strong> dollar</p> 
   <label for="tirada">Meeqo xabo rabtaa:</label> 
   <input type="number" id="tirada" value="1" min="1" onchange="xisaabiQiimaha()"> 
   <p>Wadarta lacagta: <span id="qiimahaTotal"></span> dollar</p> 
   <button onclick="goBack()">Back</button> 
   <button onclick="goToCheckout()">Dalbo Hadda</button> 
  </div> 
  <div id="checkoutPage" class="page" style="text-align: center;"> 
   <h2>Lacag Bixinta</h2> 
   <p>Waxaad dooratay: <strong id="tiradaCheckout">1</strong> x <span id="checkoutItemName"></span></p> 
   <p>Wadarta lacagta: <strong id="checkoutTotal"></strong> dollar</p> 
   <h3>Dooro Habka Lacagta:</h3> 
   <select id="paymentMethod"> <option value="Zaad">Zaad</option> <option value="Edahab">Edahab</option> <option value="Golis">Golis</option> <option value="EVC Plus">EVC Plus</option> <option value="somnet">somnet</option> </select> 
   <br> 
   <br> 
   <input type="tel" id="phoneNumber" placeholder="Geli lambarka taleefanka"> 
   <br> 
   <br> 
   <button onclick="goBackToOrder()">Back</button> 
   <button onclick="confirmPayment()">Xaqiiji Bixinta</button> 
  </div> 
  <footer> 
   <nav> 
    <a href="#">Accueil</a> 
    <a href="#">Nourriture</a> 
    <a href="#">Boissons</a> 
    <a href="#">Mon Panier</a> 
    <a href="#">Gestion</a> 
   </nav> 
  </footer> 
  <script>
    let currentItem = '';
    let currentPrice = 0;

    document.getElementById('search').addEventListener('input', function (e) {
      const query = e.target.value.toLowerCase();
      document.querySelectorAll('.card').forEach(card => {
        const text = card.innerText.toLowerCase();
        card.style.display = text.includes(query) ? 'block' : 'none';
      });
    });

    function openOrder(itemName, price, imageUrl) {
      currentItem = itemName;
      currentPrice = price;

      document.getElementById('homePage').style.display = 'none';
      document.getElementById('orderTitle').innerText = 'Dalbo ' + itemName;
      document.getElementById('itemPriceText').innerText = price;
      document.getElementById('orderImage').src = imageUrl;
      document.getElementById('orderPage').style.display = 'block';
      xisaabiQiimaha();
    }

    function goBack() {
      document.getElementById('orderPage').style.display = 'none';
      document.getElementById('homePage').style.display = 'block';
    }

    function xisaabiQiimaha() {
      const tirada = document.getElementById('tirada').value;
      const total = currentPrice * tirada;
      document.getElementById('qiimahaTotal').innerText = total.toFixed(2);
    }

    function goToCheckout() {
      const tirada = document.getElementById('tirada').value;
      const total = currentPrice * tirada;

      document.getElementById('tiradaCheckout').innerText = tirada;
      document.getElementById('checkoutTotal').innerText = total.toFixed(2);
      document.getElementById('checkoutItemName').innerText = currentItem;

      document.getElementById('orderPage').style.display = 'none';
      document.getElementById('checkoutPage').style.display = 'block';
    }

    function goBackToOrder() {
      document.getElementById('checkoutPage').style.display = 'none';
      document.getElementById('orderPage').style.display = 'block';
    }

    function confirmPayment() {
      const method = document.getElementById('paymentMethod').value;
      const number = document.getElementById('phoneNumber').value;
      const tirada = document.getElementById('tiradaCheckout').innerText;
      const total = document.getElementById('checkoutTotal').innerText;

      if (!number || number.length < 6) {
        alert("Fadlan geli lambarka telefoonka saxda ah.");
        return;
      }

      alert(`Mahadsanid!\nWaxaad dalbatay: ${tirada} x ${currentItem}\nWadarta: ${total} $\nHabka: ${method}\nLambarka: ${number}`);

      document.getElementById('checkoutPage').style.display = 'none';
      document.getElementById('homePage').style.display = 'block';
    }
  </script> 
  <meta charset="UTF-8"> 
  <title>Dalbo Burger</title> 
  <style>
    body {
      background-color: #f8f8f8;
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 50px;
    }
    .container {
      background-color: #fff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      display: inline-block;
    }
    h2 {
      color: #d35400;
      margin-bottom: 20px;
    }
    label {
      font-size: 18px;
      margin-top: 10px;
      display: block;
    }
    input[type="text"], input[type="number"] {
      padding: 10px;
      margin-top: 5px;
      width: 80%;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      background-color: #e67e22;
      color: white;
      border: none;
      padding: 12px 25px;
      margin-top: 20px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background-color: #d35400;
    }
  </style> 
  <meta charset="UTF-8"> 
  <title>Dalbo Burger</title> 
  <style>
    body {
      background-color: #fff4e6; /* oranji khafiif ah */
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 50px;
    }
    .container {
      background-color: #ffffff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      display: inline-block;
    }
    h2 {
      color: #d35400;
      margin-bottom: 20px;
    }
    label {
      font-size: 18px;
      margin-top: 10px;
      display: block;
    }
    input[type="text"], input[type="number"] {
      padding: 10px;
      margin-top: 5px;
      width: 80%;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      background-color: #e67e22;
      color: white;
      border: none;
      padding: 12px 25px;
      margin-top: 20px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background-color: #d35400;
    }
  </style>   
 </body>
</html>
