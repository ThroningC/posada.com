<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Invitación a la Posada</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 600px;
            width: 100%;
        }

        h1 {
            font-size: 2em;
            margin-bottom: 20px;
        }

        .image-container {
            width: 100%;
            height: 300px;
            background-image: url('https://via.placeholder.com/600x300'); /* Cambia por tu imagen */
            background-size: cover;
            background-position: center;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .buttons-container {
            margin: 20px 0;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 5px;
            margin: 0 10px;
        }

        button:hover {
            background-color: #45a049;
        }

        .response-image {
            display: none;
            margin-top: 20px;
            width: 100%;
            max-width: 500px;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Asistirás a la posada?</h1>
        
        <div class="image-container"></div>

        <div class="buttons-container">
            <button id="yesButton">Sí</button>
            <button id="noButton">No</button>
        </div>

        <img id="responseImage" class="response-image" src="https://via.placeholder.com/500x300?text=¡Nos+Vemos+En+La+Posada!" alt="Respuesta Positiva">
    </div>

    <script>
        // Seleccionar los botones y la imagen de respuesta
        const yesButton = document.getElementById('yesButton');
        const noButton = document.getElementById('noButton');
        const responseImage = document.getElementById('responseImage');

        // Mostrar la imagen de respuesta al hacer clic en "Sí"
        yesButton.addEventListener('click', function() {
            responseImage.style.display = 'block'; // Muestra la imagen
        });

        // Si el usuario hace clic en "No", no se muestra nada adicional
        noButton.addEventListener('click', function() {
            responseImage.style.display = 'none'; // Oculta la imagen si se hace clic en "No"
        });
    </script>

</body>
</html>
