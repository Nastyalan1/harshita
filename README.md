<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Go On A Date With Me?</title>
    <style>
        body {
            background-image: url('https://i.pinimg.com/736x/6e/2d/cf/6e2dcf7e9705bd62f3a384f222931aa9.jpg');
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            text-align: center;
            background: #ffffff;
            padding: 20px;
            border: 2px solid #9e7865;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .container h1 {
            color: #332c26;
        }
        .container button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: #382b25;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .container button:hover {
            background-color: #9e7865;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Will you go on a date with me? 🥰</h1>
        <button onclick="window.location.href='page2.html'">Yes! 💖</button>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calendar Date Picker</title>
    <style>
        body {
            background-image: url('https://i.pinimg.com/736x/1c/1f/1d/1c1f1d49086a6937f3bbc44925f2bb49.jpg');
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f4f4f9;
        }
        .container {
            text-align: center;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        #selectedDate {
            margin-top: 20px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Select a Date</h1>
        <input type="date" id="datePicker">
        <div id="selectedDate">Selected Date: None</div>
    </div>
    <script>
        const datePicker = document.getElementById('datePicker');
        const selectedDate = document.getElementById('selectedDate');
        datePicker.addEventListener('change', () => {
            const date = new Date(datePicker.value);
            const formattedDate = `${date.getDate()}/${date.getMonth() + 1}/${date.getFullYear()}`;
            selectedDate.textContent = `Selected Date: ${formattedDate}`;
        });
    </script>
    <button onclick="window.location.href='page3.html'">ALSOOO</button>
</html>

