<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>San Valentín para Ansita</title>
    <style>
        body {
            font-family: Cambria, serif;
            text-align: center;
            background-color: #ffe6e6;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            max-width: 400px;
        }
        h1, p {
            font-weight: bold;
        }
        button {
            background: #ff4d4d;
            color: white;
            border: none;
            padding: 10px 20px;
            margin: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background: #e60000;
        }
    </style>
</head>
<body>
    <div class="card" id="page1">
        <h1>Para Ansita, de Liam Tiramisú</h1>
        <p>Tengo que decirte algo, ¿querés saber el qué?</p>
        <button onclick="showPage(2)">Sí</button>
    </div>
    
    <div class="card" id="page2" style="display: none;">
        <p>Este será nuestro primer 14 de febrero juntos, bien en todos los sentidos, pero no el último. Me haría muy feliz pasarlo a tu lado juca.</p>
        <button onclick="showPage(3)">Acepto negro</button>
        <button>No</button>
    </div>

    <div class="card" id="page3" style="display: none;">
        <p>Oke, hay algo más que quiero que sepas.</p>
        <button onclick="showPage(4)">A ver</button>
    </div>

    <div class="card" id="page4" style="display: none;">
        <h1>Ansita</h1>
        <p>Quiero que sepas lo importante que eres para mí. Hemos pasado por muchas cosas en casi tres años juntos, y si hemos llegado hasta aquí, en gran parte ha sido gracias a ti. Aprecio todo lo que has hecho y todo lo que sigues haciendo por nuestra relación.</p>
        <p>Gracias por seguir a mi lado a pesar de todo. No estás sola, me tienes a mí y siempre podrás contar conmigo para lo que sea, no olvides que te amo juca❤️</p>
    </div>

    <script>
        function showPage(pageNumber) {
            document.querySelectorAll('.card').forEach(card => card.style.display = 'none');
            document.getElementById(`page${pageNumber}`).style.display = 'block';
        }
    </script>
</body>
</html>
