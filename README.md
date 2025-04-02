<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biografía Profesional</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="wrapper">
        <div class="container">
            <div class="profile">
                <img src="public/image.jpg" alt="Foto de perfil" class="profile-img">
                <div class="bio">
                    <h1>Maximiliano Medina</h1>
                    <h2>Estudiante en la Facultad de Ingeniería | Carrera: Desarrollo y Calidad de Software</h2>
                    <p>
                        Hola! soy un chico de 21 años, estoy estudiando una tecnicatura en programación en la Universidad Santo Tomás de Aquino (UNSTA) y aspiro a trabajar de eso.
                         La verdad, mi sueño es tener mi dinero, mantener a mi madre y comprarle una casa.
                         Y ademas de eso tambien planeo seguir progresando y adquirir el mayor conocmiento posible en este camino de programar y la vida.
                         
                    </p>
                </div>
            </div>
            
            <div class="experience">
                <h3>Mis Trabajos</h3>
                <ul>
                    <li>💼 Dueño de un negocio llamado "Despensa Silvia"</li>
                    <li>🎓 Estudiante en la carrera de Desarrollo y Calidad de Software</li>
                </ul>
            
            </div>
            
     <div class="companeros">
                <h2>📚 Mis Compañeros de Clase</h2>
                <ul>
                    <li>
                        <a href="https://www.instagram.com/nazarenomiguel73/?__pwa=1" target="_blank" style="color: #f0f0f0;">
                            👤 Nazareno Miguel (@nazarenomiguel73)
                        </a>
                    </li>
                    <li>
                        <a href="https://www.instagram.com/ignacio_iramain/?__pwa=1" target="_blank" style="color: #f0f0f0;">
                            👤 Iramain Ignacio (@ignacio_iramain)
                        </a>
                    </li>
                    <li>
                        <a href="https://www.instagram.com/santiago_albornoz1/?__pwa=1" target="_blank" style="color: #f0f0f0;">
                            👤 Santiago Albornoz (@santiago_albornoz1)
                        </a>
                    </li>
                    <li>
                        <a href="https://www.instagram.com/natyayusa/?__pwa=1" target="_blank"  style="color: #f0f0f0;">
                            👤 Natalia Ayusa (@natyayusa)
                        </a>
                    </li>  
                </ul>
            </div>
            
            <div class="estadoMateria">
                <h3>Materias cursadas</h3>
                <ul>
                    <li>Fundamentos del control de calidad </li>
                    <li>Desarrollo Front end</li>
                    <li>Seminario informático II</li>
                    <li>Inglés II</li>
                    <li>Formacion Humanística</li>
                </ul>
            
            </div>
            
            <link rel="stylesheet" href="styles.css">

        <body>


  <div class="table-container">
    <h2>📚 Materias y Estado</h2>
            <input type="text" id="busqueda" placeholder="Buscar materia...">
            <p id="estadoMateria"></p>
    <table>
        <thead>
            <tr>
                <th>Materia</th>
                <th>Estado</th>
            </tr>
        </thead>
        <tbody style="color:cyan">
            <tr>
                <td>Fundamentos del control de calidad</td>
                <td>Cursando</td>
            </tr>
            <tr>
                <td>Desarrollo de front end</td>
                <td>Cursando</td>
            </tr>
            <tr>
                <td>Formación Humanística</td>
                <td>Cursando</td>
            </tr>
            <tr>
                <td>Inglés II</td>
                <td>Cursando</td>
            </tr>
            <tr>
                <td>Álgebra I</td>
                <td>Recursando</td>
            </tr>
        </tbody>
    </table>
</div>

            <title>Mis Redes</title>
            <style>
                body { 
                    font-family: Arial, sans-serif; 
                    text-align: center; 
                    background-color: #f0f0f0; 
                    padding: 20px; 
                }
                .contenedor {
                    background-color: white;
                    width: 50%;
                    margin: auto;
                    padding: 20px;
                    border-radius: 10px;
                    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
                }
                .redes {
                    font-size: 20px;
                    margin-top: 10px;
                }
                a {
                    display: inline-block;
                    font-size: 18px;
                    color: #007BFF;
                    text-decoration: none;
                    font-weight: bold;
                    margin-top: 5px;
                }
                a:hover { 
                    color: #0056b3; 
                }
            </style>
        <body>
        
            <div class="contenedor">
                <h2>Mis Redes</h2>
        
                <p class="redes">
                    📷 Instagram:  
                    <a href="https://www.instagram.com/maxi_medina03/?__pwa=1" target="_blank">
                        @maxi_medina03
                    </a>
                </p>
        
                <p class="redes">
                    📱 WhatsApp:  
                    <a href="https://wa.me/3865506528" target="_blank">
                        Chatear en WhatsApp
                    </a>
                </p>

</body>
</html>

<script>
    document.addEventListener("DOMContentLoaded", function () {
        document.getElementById("busqueda").addEventListener("keyup", filtrarMaterias);
    });

    function filtrarMaterias() {
        let input = document.getElementById("busqueda").value; // Selecciona el input correcto
        let filas = document.querySelectorAll("tbody tr");
        let estadoTexto = document.getElementById("estadoMateria");
        let encontrado = false;

        filas.forEach(fila => {
            let materia = fila.cells[0].textContent.toLowerCase(); // Ahora usa la celda correcta
            let estado = fila.cells[1].textContent; // La segunda columna tiene el estado
            
            if (materia.includes(input) && input !== "") {
                fila.style.display = "";
                estadoTexto.textContent = "Estado: " + estado;
                encontrado = true;
            } else {
                fila.style.display = "none";
            }
        });

        if (!encontrado) {
            estadoTexto.textContent = "";
        }
    }

    </script>

                <style>
                body { font-family: Arial, sans-serif; text-align: center; background-color: #f0f0f0; }
                table { width: 100%; margin: 20px auto; border-collapse: collapse; background: white; border-radius: 10px; overflow: hidden; box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); }
                th, td { border: 1px solid black; padding: 10px; text-align: left; }
                th { background-color: #007BFF; color: white; }
                input {
                    width: 100%;
                    max-width: 600px;
                    padding: 10px;
                    margin: 10px;
                    border: 2px solid #007BFF;
                    border-radius: 5px;
                    outline: none;
                    font-size: 16px;
                }
                input:focus {
                    border-color: #0056b3;
                }
                #estadoMateria {
            font-size: 18px;
            margin-top: 10px;
            font-weight: bold;
            color: #333;
        }

        
            </style>


            <style>
    body { 
        font-family: Arial, sans-serif; 
        background-color: #f4f4f9; 
        text-align: center;
        padding: 20px;
    }

    .table-container {
        max-width: 700px;
        margin: auto;
        background: white;
        padding: 20px;
        border-radius: 12px;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
    }

    table {
        width: 100%;
        border-collapse: collapse;
        margin-top: 10px;
        border-radius: 8px;
        overflow: hidden;
    }

    th, td {
        padding: 12px;
        text-align: center;
    }

    thead {
        background-color: #007BFF;
        color: blue;
    }

    tbody tr:nth-child(even) {
        background-color: #f2f2f2;
    }

    tbody tr:hover {
        background-color: #d6e4ff;
        transition: background 0.3s;
    }

    th {
        font-weight: bold;
    }
</style>
  