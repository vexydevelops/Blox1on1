# Blox1on1
this is a 50/50 coin flip adopt me gambling website 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coin Flip</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Coin Flip</h1>
        <button id="flipBtn">Flip Coin</button>
        <p id="result"></p>
    </div>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
}

.container {
    text-align: center;
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}

#result {
    font-size: 18px;
    font-weight: bold;
    margin-top: 20px;
}
document.getElementById('flipBtn').addEventListener('click', function () {
    // Generate a random number (0 or 1)
    const randomNumber = Math.floor(Math.random() * 2);

    // Display the result
    const resultElement = document.getElementById('result');
    if (randomNumber === 0) {
        resultElement.textContent = 'Heads!';
    } else {
        resultElement.textContent = 'Tails!';
    }
});
