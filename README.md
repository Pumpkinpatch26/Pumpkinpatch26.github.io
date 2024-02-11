<!DOCTYPE html>
<html>
<head>
    <title>Valentine's Day Card</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: pink;
            text-align: center;
            padding: 50px;
            position: relative;
            height: 100vh;
            box-sizing: border-box;
        }
        #message {
            font-size: 2em;
        }
        .button {
            background-color: red;
            color: white;
            border: none;
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            cursor: pointer;
            position: relative;
        }
    </style>
</head>
<body>

<h1 id="message">Will you be my Valentine, Felicia Goh Li Lin?</h1>

<img src="https://i.ibb.co/mXDynSN/Whats-App-Image-2024-02-11-at-15-30-53-dd1be4ff.jpg" alt="A special moment">

<button class="button" onclick="responseYes()">Yes!</button>
<button id="noButton" class="button" onclick="responseNo()">Ew No!</button>

<script>
        function responseYes() {
            document.getElementById("message").innerHTML = "You, Felicia Goh Li Lin, are now Indra Raiyan Putera's valentine for February 14th, 2024!";
            document.body.style.backgroundColor = "yellow";
        }
        function responseNo() {
            var noButton = document.getElementById("noButton");
            var x = Math.random() * (window.innerWidth - noButton.offsetWidth);
            var y = Math.random() * (window.innerHeight - noButton.offsetHeight);
            noButton.style.left = x + "px";
            noButton.style.top = y + "px";
            noButton.style.position = "absolute";
        }
    </script>

</body>
</html>
