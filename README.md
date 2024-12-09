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

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>What to Eat?</title>
    <style>
        body {
            background-image: url('https://i.pinimg.com/736x/5d/8a/a3/5d8aa361011a48fb147e7993b6ce9dcc.jpg');
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            background-color: #f8f8f8;
        }
        h1 {
            margin-bottom: 20px;
        }
        .food-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            max-width: 800px;
            width: 100%;
        }
        .food-item {
            position: relative;
            cursor: pointer;
            overflow: hidden;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }
        .food-item:hover {
            transform: scale(1.05);
        }
        .food-item img {
            width: 100%;
            height: auto;
            display: block;
            border-radius: 10px;
        }
        .food-item input {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            opacity: 0;
            cursor: pointer;
        }
        .food-item.selected {
            border: 5px solid #007bff;
        }
    </style>
</head>
<body>
    <h1>What would you like to eat?</h1>
    <div class="food-gallery">
        <label class="food-item">
            <img src="https://i.pinimg.com/736x/70/77/16/7077161cdb252c166a4ac4be69a59760.jpg" alt="Pani puri">
            <input type="radio" name="food" value="Pizza">
        </label>
        <label class="food-item">
            <img src="https://i.pinimg.com/736x/d3/42/1f/d3421fedf1f7648ca7c7f1879c397c4b.jpg" alt="Burger">
            <input type="radio" name="food" value="Burger">
        </label>
        <label class="food-item">
            <img src="https://i.pinimg.com/736x/27/e9/b3/27e9b396a2d11d82f85337742e380dc6.jpg" alt="Sushi">
            <input type="radio" name="food" value="Sushi">
        </label>
        <label class="food-item">
            <img src="https://i.pinimg.com/736x/a9/4e/49/a94e49fc39e6a12d7b3b8d713b07767a.jpg" alt="Ice Cream">
            <input type="radio" name="food" value="Ice Cream">
        </label>
    </div>
    <script>
        const items = document.querySelectorAll('.food-item');
        items.forEach(item => {
            item.addEventListener('click', () => {
                items.forEach(i => i.classList.remove('selected'));
                item.classList.add('selected');
            });
        });
    </script>
     <button onclick="window.location.href='page4.html'">Yes! 💖</button>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Date Place Selector</title>
    <style>
        body {
            background-image: url('https://i.pinimg.com/736x/49/86/45/498645a3da87e7ce0325f68fb5bb81cc.jpg');
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            padding: 20px;
            background-color: #ffffff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        .images {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }
        .image-item {
            width: 150px;
            height: 150px;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .image-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        label, select {
            display: block;
            margin: 20px auto;
            text-align: center;
            font-size: 16px;
        }
        select {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f1f1f1;
            font-size: 16px;
        }
        button {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            background-color: #007BFF;
            color: #ffffff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <label for="places">Choose a place to visit:</label>
        <div class="images">
            <div class="image-item">
                <img src="https://i.pinimg.com/736x/bb/c9/72/bbc972d009c77a0e0dd316fbc62e72b8.jpg" alt="Beautiful Park">
            </div>
            <div class="image-item">
                <img src="https://i.pinimg.com/736x/e1/76/43/e176438d47b8c7e278d79aa51c0c3991.jpg" alt="Art Museum">
            </div>
            <div class="image-item">
                <img src="https://i.pinimg.com/736x/c2/6b/1c/c26b1c52457b9418de5929f1a2734f96.jpg" alt="Sunny Beach">
            </div>
            <div class="image-item">
                <img src="https://i.pinimg.com/736x/82/81/04/8281048cf5f30a817bbd79280951a845.jpg" alt="Movie Theater">
            </div>
        </div>
    </div>
    <script>
        function submitChoice() {
            const selectedPlace = document.getElementById('places').value;
            alert(`You chose to visit: ${selectedPlace}`);
        }
    </script>
     <button onclick="window.location.href='page5.html'">And alsoooo</button>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Can We Hold Hands?</title>
    <style>
        body {
            background-image: url('https://i.pinimg.com/736x/91/e1/33/91e133ec0bbbdbab7e81ae937ac9def7.jpg'); /* Replace with the desired image URL */
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            color: white;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }
        .container {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
            border-radius: 10px;
        }
        button {
            background-color: #4CAF50; /* Green */
            border: none;
            color: white;
            padding: 10px 20px;
            margin: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color:  #ff0000; /* Darker green */
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Can we also hold hands?</h1>
        <button onclick="alert('You clicked Yes!')">Yes</button>
        <button onclick="alert('You clicked No!')">No</button>  
    </div>
    <button onclick="window.location.href='page6.html'"> AND alsooo</button> 
</body>

</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thank You</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #f0f8ff;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 3em;
            color: #ff6347;
            text-align: center;
            z-index: 10;
        }
        .heart {
            position: absolute;
            top: -50px;
            font-size: 3em;
            color: red;
            animation: fall 5s infinite;
        }
        @keyframes fall {
            0% {
                transform: translateY(0) rotate(0deg);
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
            }
        }
        .heart:nth-child(odd) {
            animation-duration: 5s;
        }
        .heart:nth-child(even) {
            animation-duration: 6s;
        }
    </style>
</head>
<body>
    <h1>Thank you for being with me! 💖</h1>
    <div class="heart" style="left: 10%;">❤️</div>
    <div class="heart" style="left: 20%;">❤️</div>
    <div class="heart" style="left: 30%;">❤️</div>
    <div class="heart" style="left: 40%;">❤️</div>
    <div class="heart" style="left: 50%;">❤️</div>
    <div class="heart" style="left: 60%;">❤️</div>
    <div class="heart" style="left: 70%;">❤️</div>
    <div class="heart" style="left: 80%;">❤️</div>
    <div class="heart" style="left: 90%;">❤️</div>


</body>
</html>
