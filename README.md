# green-and-red-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Red-Green Toggle Button</title>
  <style>
    /* Center the button on the page */
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background: #f0f0f0;
    }

    /* Style the button */
    #colorToggle {
      padding: 12px 24px;
      font-size: 18px;
      font-family: sans-serif;
      background-color: red;
      color: #fff;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
  </style>
</head>
<body>

  <button id="colorToggle">Red</button>

  <script>
    const btn = document.getElementById('colorToggle');
    let isRed = true;

    btn.addEventListener('click', () => {
      if (isRed) {
        btn.style.backgroundColor = 'green';
        btn.textContent = 'Green';
      } else {
        btn.style.backgroundColor = 'red';
        btn.textContent = 'Red';
      }
      isRed = !isRed;
    });
  </script>

</body>
</html>
