<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scientific Number Check</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: #b0b0b0; /* Warna abu-abu */
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .container {
            background: #f28b82; /* Warna merah lembut */
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
            width: 350px;
        }
        h2, p {
            margin: 10px 0;
            color: white;
        }
        input {
            width: 80%;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: white;
            color: black;
            padding: 10px 20px;
            font-size: 16px;
            border: 1px solid black;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: #e0e0e0;
        }
        .result {
            margin-top: 15px;
            font-size: 18px;
            font-weight: bold;
            color: white;
        }
        .author {
            margin-top: 20px;
            padding: 10px;
            font-size: 16px;
            font-weight: bold;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Scientific Number Check</h2>
        <p>Please Enter a Number</p>
        <input type="text" id="numberInput" placeholder="Type your number here...">
        <button onclick="checkNumber()">Check</button>
        <p class="result" id="result">Waiting for input...</p>
        <div class="author">
            Marcelino Winowoda<br>221011060047
        </div>
    </div>

    <script>
        function checkNumber() {
            let input = document.getElementById("numberInput").value.trim();
            
            if (input === "" || isNaN(input)) {
                document.getElementById("result").innerText = "No, it is not a number";
                return;
            }

            document.getElementById("result").innerText = "Yes, it is a number";
        }
    </script>
</body>
</html>


            document.getElementById("result").innerText = "Yes, it is a number";
        }
    </script>
</body>
</html>
