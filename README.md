# me-perdonas
<!DOCTYPE html>
<html>
<head>
    <title>Me perdonas</title>
    <style>
        #options {
            display: none;
        }
        #yesButton, #noButton {
            margin: 5px;
        }
    </style>
</head>
<body>
    <a href="#" onclick="showOptions(); return false;">me perdonas</a>
    <div id="options">
        <button id="yesButton" onclick="sayThankYou()">Sí</button>
        <button id="noButton" onclick="enlargeNo()">No</button>
    </div>
    <div id="message"></div>

    <script>
        function showOptions() {
            document.getElementById('options').style.display = 'block';
        }

        function sayThankYou() {
            document.getElementById('message').innerHTML = '¡Gracias, te quiero!';
            document.getElementById('options').style.display = 'none';
        }

        function enlargeNo() {
            document.getElementById('yesButton').style.fontSize = '24px';
            document.getElementById('noButton').style.fontSize = '12px';
        }
    </script>
</body>
</html>