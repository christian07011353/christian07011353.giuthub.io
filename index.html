<?php
$host = "localhost";
$username = "christian";
$password = "hachi1";
$database = "hotel_db";

// Conexión a la base de datos
$connection = mysqli_connect($host, $username, $password, $database);

// Verificar la conexión
if (!$connection) {
    die("No se ha podido conectar con la base de datos: " . mysqli_connect_error());
} else {
    echo "Conexión exitosa a la base de datos";
}

// Verificar si se ha enviado el formulario
if (isset($_SERVER["REQUEST_METHOD"]) && $_SERVER["REQUEST_METHOD"] == "POST") {
    // Recuperar los datos del formulario
    $nombre_apellido = isset($_POST['nombre_apellido']) ? $_POST['nombre_apellido'] : '';
    $fecha_entrada = isset($_POST['fecha_entrada']) ? $_POST['fecha_entrada'] : '';
    $fecha_salida = isset($_POST['fecha_salida']) ? $_POST['fecha_salida'] : '';
    $personas = isset($_POST['personas']) ? $_POST['personas'] : '';
    $tipo_habitacion = isset($_POST['tipo_habitacion']) ? $_POST['tipo_habitacion'] : '';
    $metodo_pago = isset($_POST['metodo_pago']) ? $_POST['metodo_pago'] : '';
    $email = isset($_POST['email']) ? filter_var($_POST['email'], FILTER_SANITIZE_EMAIL) : '';

    // Validar el correo electrónico
    $email_valido = filter_var($email, FILTER_VALIDATE_EMAIL);
    if ($email_valido) {
        // El correo electrónico es válido
        echo "El correo electrónico ingresado es válido: $email";

        // Consulta SQL para insertar datos en la tabla 'reservas'
        $instruccion_SQL = "INSERT INTO reservas (nombre_apellido, fecha_entrada, fecha_salida, personas, tipo_habitacion, metodo_pago, email) 
                            VALUES ('$nombre_apellido', '$fecha_entrada', '$fecha_salida', '$personas', '$tipo_habitacion', '$metodo_pago', '$email')";
        
        // Ejecutar la consulta
        if (mysqli_query($connection, $instruccion_SQL)) {
            echo "Datos insertados correctamente";
        } else {
            echo "No se ha podido insertar los datos: " . mysqli_error($connection);
        }
    } else {
        // El correo electrónico no es válido
        echo "El correo electrónico ingresado no es válido";
    }
} else {
    // Esto se ejecutará si el formulario no se ha enviado por POST
    // Por ejemplo, cuando el usuario accede a la página directamente
    echo "Esperando el envío del formulario...";
}

// Cerrar la conexión
mysqli_close($connection);
?>

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario de Reserva de Hotel</title>
    <link rel="stylesheet" href="feo.css">
</head>

<body>
    <h2>Formulario de Reserva de Hotel</h2>
    <form action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]); ?>" method="post">
        <label for="nombre_apellido">Nombre y Apellido:</label>
        <input type="text" id="nombre_apellido" name="nombre_apellido" required><br><br>

        <label for="fecha_entrada">Fecha de Entrada:</label>
        <input type="date" id="fecha_entrada" name="fecha_entrada" required><br><br>

        <label for="fecha_salida">Fecha de Salida:</label>
        <input type="date" id="fecha_salida" name="fecha_salida" required><br><br>

        <label for="personas">Número de Personas:</label>
        <input type="number" id="personas" name="personas" required><br><br>

        <label for="tipo_habitacion">Tipo de Habitación:</label>
        <select id="tipo_habitacion" name="tipo_habitacion" required>
            <option value="individual">Individual</option>
            <option value="doble">Doble</option>
            <option value="suite">Suite</option>
            <option value="economica">Economica</option>
            <option value="familiar">Familiar</option>
            <option value="para dos">Para dos</option>
        </select><br><br>

        <label for="metodo_pago">Método de Pago:</label>
        <select id="metodo_pago" name="metodo_pago" required>
            <option value="tarjeta">Tarjeta de Crédito</option>
            <option value="efectivo">Efectivo</option>
            <option value="transferencia">Transferencia Bancaria</option>
        </select><br><br>

        <label for="email">Correo Electrónico:</label>
        <input type="email" id="email" name="email" required><br><br>

        <input type="submit" value="Enviar Reserva">
        <input type="reset" value="Restablecer">
    </form>
</body>
</html>







