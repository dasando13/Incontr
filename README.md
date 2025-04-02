<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Incontra il Professionista</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000;
            color: white;
        }
        header {
            background-color: #ff6600;
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 20px;
            font-weight: bold;
            text-transform: uppercase;
        }
        .menu-icon {
            font-size: 24px;
            cursor: pointer;
        }
        .sidebar {
            position: fixed;
            left: -250px;
            top: 0;
            width: 250px;
            height: 100%;
            background: #111;
            transition: 0.3s;
            padding-top: 60px;
        }
        .sidebar a {
            padding: 10px 20px;
            text-decoration: none;
            color: white;
            display: block;
            text-transform: uppercase;
        }
        .sidebar a:hover {
            background: #ff6600;
        }
        .close-btn {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 30px;
            cursor: pointer;
        }
        .content {
            padding: 20px;
            text-align: center;
        }
        .content img {
            max-width: 100%;
            border-radius: 10px;
        }
    </style>
    <script>
        function openMenu() {
            document.getElementById("sidebar").style.left = "0";
        }
        function closeMenu() {
            document.getElementById("sidebar").style.left = "-250px";
        }
    </script>
</head>
<body>
    <header>
        <div class="logo">INCONTRA IL PROFESSIONISTA</div>
        <div class="menu-icon" onclick="openMenu()">☰</div>
    </header>
    <div id="sidebar" class="sidebar">
        <div class="close-btn" onclick="closeMenu()">×</div>
        <a href="#">Home</a>
        <a href="#">Chi Siamo</a>
        <a href="#">Contatti</a>
    </div>
    <div class="content">
        <h1>Dalla Scuola al Successo</h1>
        <img src="school-success.jpg" alt="Scuola al successo">
        <p>Cos'è "Incontra il Professionista"?</p>
    </div>
</body>
</html>
