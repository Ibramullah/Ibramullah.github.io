<!DOCTYPE html>
<html>
<head>
  <title>Cafe Menu</title>
  <style>

    /* Body Page */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Home Page */
    header {
      background-color: #333;
      color: #fff;
      padding: 20px;
      text-align: center;
    }

    /* Main Page */
    main {
      padding: 40px;
      text-align: center;
    }

    /* Button */
    .buttons-container {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 50px;
    }

    .btn {
      background-color: #fff;
      border: 2px solid #1b4169;
      color: #ffffff;
      padding: 45px 165px;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      position: relative;
      z-index: 1;
      font-size: 24px;
    }

    .btn:before {
      content: "";
      background-size: cover;
      background-position: center;
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      z-index: -1;
    }

    .btn-indoor:before {
      background-image: url("https://images.unsplash.com/photo-1554118811-1e0d58224f24?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8Y2FmZXxlbnwwfHwwfHx8MA%3D%3D&w=1000&q=80");
    }

    .btn-outdoor:before {
      background-image: url("https://awsimages.detik.net.id/community/media/visual/2022/06/26/cafe-di-makassar-yang-mengusung-konsep-taman_169.jpeg?w=650&q=80");
    }

    /* Devider */
    .divider {
      width: 100%;
      height: 2px;
      background-color: #ccc;
      margin-top: 50px;
      margin-bottom: 30px;
    }

    /* Header Selection */
    .h1-selection {
        font-family: Arial, sans-serif;
      margin-left: 40px;
      padding: 10;
    }

    /* Cafe Selection Page */
    .menu-item {
      display: flex;
      align-items: center;
      cursor: pointer;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
      padding: 10px;
    }

    .menu-item:hover {
      background-color: #f9f9f9;
    }

    .menu-item img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      border-radius: 5px;
      margin-right: 10px;
    }

    .menu-item .content {
      flex-grow: 1;
    }

    .menu-item .name {
      font-weight: bold;
      font-size: 20px;
    }

    .menu-item .description {
      font-size: 14px;
      margin-top: 5px;
      color: #888;
    }

    /* Expended Information */
    .menu-item .expanded-info {
      display: none;
      margin-top: 10px;
      padding: 10px;
      background-color: #f9f9f9;
      border-radius: 5px;
      font-size: 14px;
      line-height: 1.5;
    }

    .menu-item.expanded .expanded-info {
      display: block;
    }

    /* Footer */
    footer {
      background-color: #f9f9f9;
      padding: 10px;
      text-align: center;
      font-size: 12px;
      color: #888;
    }


  </style>
</head>


<body>
  <header>
        <!-- Home Page -->
        <h1>Café Location Guide</h1>
        <h2>Indoor</h2>
        <p></p>
        <p></p>
  </header>

   <!-- Header Cafe Selection -->
  <div class="h1-selection">
    <h1>Cafe Selection</h1>
    </div>
  
  <!-- Cafe Selection -->
  <main>
     <div class="menu-item">
      <img src="image1.jpg" alt="Item 1">
      <div class="content">
          <div class="name">Item 1</div>
         <div class="description">Mini description for Item 1</div>
         <div class="expanded-info">
           More information about Item 1, including ingredients, preparation method, and price.
          </div>
     </div>
     </div>

     <div class="menu-item">
       <img src="image2.jpg" alt="Item 2">
       <div class="content">
          <div class="name">Item 2</div>
          <div class="description">Mini description for Item 2</div>
         <div class="expanded-info">
           More information about Item 2, including ingredients, preparation method, and price.
          </div>
     </div>
     </div>

     <div class="menu-item">
     <img src="image3.jpg" alt="Item 3">
      <div class="content">
          <div class="name">Item 3</div>
          <div class="description">Mini description for Item 3</div>
         <div class="expanded-info">
           More information about Item 3, including ingredients, preparation method, and price.
          </div>
     </div>
     </div>

     <div class="menu-item">
      <img src="image4.jpg" alt="Item 4">
      <div class="content">
          <div class="name">Item 4</div>
          <div class="description">Mini description for Item 4</div>
          <div class="expanded-info">
            More information about Item 4, including ingredients, preparation method, and price.
       </div>
     </div>
      </div>

     <div class="menu-item">
      <img src="image5.jpg" alt="Item 5">
      <div class="content">
          <div class="name">Item 5</div>
          <div class="description">Mini description for Item 5</div>
          <div class="expanded-info">
           More information about Item 5, including ingredients, preparation method, and price.
          </div>
     </div>
    </div>
    
    </main>

  <footer>
    <p>&copy; 2023 Café Location Guide. All rights reserved.</p>
  </footer>

  <script>
    const menuItems = document.querySelectorAll('.menu-item');

    menuItems.forEach(item => {
      item.addEventListener('click', () => {
        item.classList.toggle('expanded');
      });
    });
  </script>


</body>
</html>
