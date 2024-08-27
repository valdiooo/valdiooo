- 👋 Hi, I’m @valdiooo
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
valdiooo/valdiooo is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tebak Angka Game By Valdioo</title>
    <style>
    <title>Kalo 1X coba Langsung benar ku kasih 2k! </title>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            margin: 0;
        }
        .game-container {
            text-align: center;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        input {
            padding: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px;
            font-size: 16px;
            cursor: pointer;
        }
        .message {
            margin-top: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="game-container">
        <h1>Tebak Angka By valdioo kalo langsung benar kukasih 2k sambil video yaa</h1>
        <p>Tebak angka antara 1 dan 100:</p>
        <input type="number" id="guess" min="1" max="1000">
        <button onclick="checkGuess()">Tebak</button>
        <div class="message" id="message"></div>
    </div>

    <script>
        // Menghasilkan angka acak antara 1 dan 10
        let secretNumber = Math.floor(Math.random() * 10) + 1;

        function checkGuess() {
            const guess = parseInt(document.getElementById('guess').value);
            const messageElement = document.getElementById('message');

            if (guess === secretNumber) {
                messageElement.textContent = 'Selamat! Anda benar!';
                messageElement.style.color = 'green';
            } else {
                messageElement.textContent = 'Salah! Coba lagi.';
                messageElement.style.color = 'red';
            }
        }
    </script>
</body>
</html>

