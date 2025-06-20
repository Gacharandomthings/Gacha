<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test gacha số</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            text-align: center;
            padding: 50px;
        }
        .container {
            max-width: 400px;
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #333;
        }
        button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #0056b3;
        }
        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Trò Chơi Số Ngẫu Nhiên</h1>
        <button onclick="generateRandomNumber()">Ấn bố mày đê!</button>
        <p id="result"></p>
    </div>
    <script>
        function generateRandomNumber() {
            // Hiển thị thông báo chờ
            document.getElementById("result").innerText = "Bố mày đang bốc số chờ tí...";
            // Tạo số ngẫu nhiên và hiển thị sau 1,05 giây
            setTimeout(() => {
                const randomNumber = Math.floor(Math.random() * 10) + 1;
                document.getElementById("result").innerText = `Mày đã trúng ${randomNumber}`;
            }, 1050); // Độ trễ 1050ms = 1,05 giây
        }
    </script>
</body>
</html>
