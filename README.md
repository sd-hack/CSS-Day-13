# CSS-Day-13
<!DOCTYPE html>
<html>
<head>
  <title>Responsive Cards</title>
  <style>
    body {
      margin: 0;
      padding: 20px;
      background: #f2f2f2;
      font-family: Arial, sans-serif;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    /* Card Container */
    .card-container {
      display: grid;
      grid-template-columns: repeat(3, 1fr); /* Desktop: 3 cards */
      gap: 20px;
      max-width: 1000px;
      margin: auto;
    }

    /* Card Style */
    .card {
      background: white;
      padding: 20px;
      border-radius: 8px;
      text-align: center;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .card h3 {
      margin-top: 0;
    }

    /* Tablet: 2 cards per row */
    @media (max-width: 900px) {
      .card-container {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    /* Mobile: stack vertically */
    @media (max-width: 600px) {
      .card-container {
        grid-template-columns: 1fr;
      }
    }

  </style>
</head>

<body>

  <h2>My Content Cards</h2>

  <div class="card-container">
    <div class="card">
      <h3>Card 1</h3>
      <p>This is the first content card.</p>
    </div>

    <div class="card">
      <h3>Card 2</h3>
      <p>This is the second content card.</p>
    </div>

    <div class="card">
      <h3>Card 3</h3>
      <p>This is the third content card.</p>
    </div>
  </div>

</body>
</html>
