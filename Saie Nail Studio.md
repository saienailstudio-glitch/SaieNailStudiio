# Saie Nail Studio   
<!DOCTYPE html>  
<html lang="es">  
<head>  
<meta charset="UTF-8">  
<title>Saie Nail Studio</title>  
<style>  
body {  
    font-family: Arial;  
    background-color: #f5efe6;  
    text-align: center;  
    color: #4b3832;  
}  
.container {  
    background: white;  
    padding: 20px;  
    margin: 20px auto;  
    width: 90%;  
    max-width: 400px;  
    border-radius: 10px;  
}  
input, select, button {  
    width: 90%;  
    padding: 10px;  
    margin: 10px;  
}  
button {  
    background: #8d6e63;  
    color: white;  
    border: none;  
}  
</style>  
</head>  
<body>  
<h2>Saie Nail Studio 💅</h2>  
<div class="container">  
<input type="text" id="nombre" placeholder="Tu nombre">  
<input type="date" id="fecha">  
<select id="servicio">  
<option>Uñas acrílicas</option>  
<option>Baño de acrílico</option>  
<option>Nivelación Rubber Gel</option>  
<option>Retoque de uñas</option>  
<option>Retiro de uñas o gel</option>  
</select>  
<select id="hora">  
<option>Selecciona horario</option>  
<option>12:30</option>  
<option>13:00</option>  
<option>14:00</option>  
<option>15:00</option>  
<option>16:00</option>  
<option>17:00</option>  
<option>18:00</option>  
<option>18:30</option>  
</select>  
</div>  
<script>  
function enviar() {  
    let nombre = document.getElementById("nombre").value;  
    let fecha = document.getElementById("fecha").value;  
    let servicio = document.getElementById("servicio").value;  
    let hora = document.getElementById("hora").value;  
  
    let mensaje = `Hola, soy ${nombre}. Quiero agendar cita el ${fecha} a las ${hora} para ${servicio}`;  
    let url = `https://wa.me/523339003810?text=${encodeURIComponent(mensaje)}`;  
  
    window.open(url, "_blank");  
}  
</script>  
</body>  
</html>  
:::  
