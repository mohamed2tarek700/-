<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>المسبحة الإلكترونية</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
            background-color: #f4f4f4;
        }
        h1 {
            color: #008080;
        }
        .counter {
            font-size: 48px;
            color: #333;
            margin: 20px 0;
        }
        .button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            color: #fff;
            background-color: #008080;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button.reset {
            background-color: #ff5252;
        }
        .button:hover {
            opacity: 0.9;
        }
    </style>
</head>
<body>
    <h1>المسبحة الإلكترونية</h1>
    <div class="counter" id="counter">0</div>
    <button class="button" onclick="increment()">تسبيح</button>
    <button class="button reset" onclick="resetCounter()">إعادة تعيين</button>

    <script>
        let count = 0;

        function increment() {
            count++;
            document.getElementById("counter").innerText = count;
        }

        function resetCounter() {
            count = 0;
            document.getElementById("counter").innerText = count;
        }
    </script>
</body>
</html>
