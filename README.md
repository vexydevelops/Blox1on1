<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Welcome to My Website!</h1>
    </header>
    <main>
        <p>This is a simple webpage created with HTML, CSS, and JavaScript.</p>
        <button id="clickMeButton">Click me!</button>
        <p id="outputMessage"></p>
    </main>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f2f2f2;
}

header {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
}

main {
    max-width: 800px;
    margin: 20px auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}

#outputMessage {
    font-size: 18px;
    font-weight: bold;
    margin-top: 20px;
}
document.getElementById('clickMeButton').addEventListener('click', function () {
    document.getElementById('outputMessage').textContent = 'Button clicked!';
});
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
