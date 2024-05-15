<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Carta de Aniversario</title>
<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f7f7f7;
        color: #333;
    }

    .container {
        max-width: 600px;
        margin: 20px auto;
        background-color: #fff;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    h1 {
        text-align: center;
        color: #ff5e62;
    }

    p {
        line-height: 1.6;
    }

    .signature {
        text-align: center;
        margin-top: 20px;
    }

    .signature img {
        width: 100px;
        border-radius: 50%;
        margin-top: 10px;
    }

    @media (max-width: 600px) {
        .container {
            margin: 10px;
            padding: 15px;
        }

        h1 {
            font-size: 1.5em;
        }

        .signature img {
            width: 80px;
        }
    }
</style>
</head>
<body>

<noscript>Por favor, habilita JavaScript para una mejor experiencia.</noscript>

<div class="container">
    <h1>¡Feliz Aniversario!</h1>
    <p>Querido Pollito,</p>
    <p>Hoy celebramos otro mes juntas, y quiero aprovechar esta oportunidad para expresarte cuánto significas para mí. Cada día a tu lado es un regalo, y no puedo imaginar mi vida sin ti.</p>
    <p>Gracias por ser mi compañera, mi amiga y mi amor. Tu apoyo incondicional y tu amor sincero hacen que cada momento sea especial. Juntas hemos pasado por altibajos, pero siempre hemos salido más fuertes y más unidas.</p>
    <p>Estoy agradecida por todos los recuerdos que hemos creado juntas y emocionada por todos los momentos que aún tenemos por delante. Eres mi casita, mi alegría y mi razón para sonreír cada día.</p>
    <p>En este día especial, quiero renovar mi compromiso de amarte, apoyarte y cuidarte en cada paso del camino. Espero que este año esté lleno de amor, risas y momentos inolvidables para nosotras.</p>
    <p>¿QUIERES VOLVER A CASARTE CONMIGO?</p>
    <form id="casarseForm">
        <input type="radio" id="si" name="casarse" value="si">
        <label for="si">SI</label><br>
        <input type="radio" id="no" name="casarse" value="no">
        <label for="no">NO</label><br>
        <button type="submit">Enviar</button>
    </form>
    <div class="signature">
    <p>Patito</p>
    </div>
</div>

<script>
    const form = document.getElementById('casarseForm');
    let counter = 0;
    form.addEventListener('submit', function(event) {
        event.preventDefault();
        const respuesta = document.querySelector('input[name="casarse"]:checked').value;
        if (respuesta === "si") {
            alert("Perfecto, ahora no hay devolución. Debes mantenerme, darme amor y tenerme paciencia.");
        } else {
            if (counter === 0) {
                alert("¿Estás segura?");
            } else if (counter === 1) {
                alert("¿Estás completamente segura?");
            } else {
                alert("Ja, por más que digas que no, no te libras de mí.");
            }
            counter++;
        }
    });
</script>

</body>
</html>
