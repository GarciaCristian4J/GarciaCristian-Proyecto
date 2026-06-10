<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Consultorio Feliz</title>
    <style>
        /* Variables de color para cambiar todo rápido */
        :root {
            --principal: #584ca5;
            --secundario: #6e68bb;
            --fondo: #f4f4f9;
            --texto: #333;
            --blanco: #ffffff;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background-color: var(--fondo);
            color: var(--texto);
        }

        /* Header con imagen de fondo */
        header {
            background: linear-gradient(rgba(88, 76, 165, 0.8), rgba(88, 76, 165, 0.8)), 
                        url('https://images.unsplash.com/photo-1505751172107-160a0f0237a3?auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 240px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: var(--blanco);
            text-align: center;
            padding: 20px;
            gap: 12px;
        }

        header h1 {
            font-size: 2.6rem;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
        }

        /* Barra de navegación horizontal */
        .nav-horizontal {
            width: 100%;
            display: flex;
            justify-content: center;
            margin-top: -30px;
            padding: 0 20px;
        }

        .nav-horizontal ul {
            display: flex;
            gap: 10px;
            list-style: none;
            background: rgba(110, 104, 187, 0.95);
            padding: 10px 14px;
            border-radius: 999px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.12);
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-horizontal ul li a {
            display: inline-block;
            padding: 8px 12px;
            border-radius: 999px;
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            transition: 0.2s;
        }

        .nav-horizontal ul li a:hover {
            background: rgba(0,0,0,0.18);
        }


        /* Contenedor principal con Flexbox */
        .contenedor {
            display: flex;
            max-width: 1200px;
            margin: 20px auto;
            gap: 20px;
            padding: 0 20px;
            align-items: flex-start;
        }

        /* Aside (barra lateral) */
        aside.aside {
            flex: 1;
            background: var(--secundario);
            padding: 20px;
            border-radius: 10px;
            color: #fff;
            min-width: 260px;
        }

        aside.aside h3 {
            margin-bottom: 15px;
            border-bottom: 1px solid rgba(255,255,255,0.3);
            padding-bottom: 10px;
        }

        aside.aside ul {
            list-style: none;
            margin-bottom: 18px;
            width: 100%;
        }

        aside.aside ul img {
            width: 100%;
            height: auto;
            display: block;
            border-radius: 8px;
            margin-top: 10px;
        }


        aside.aside ul li {
            margin-bottom: 10px;
        }

        aside.aside a {
            color: #fff;
            text-decoration: none;
            transition: 0.2s;
        }

        aside.aside a:hover {
            color: #d1d1d1;
        }


        nav {
            display: none;
        }

        /* Contenido principal */

        /* Contenedor en línea (aside + article) */
        .contenedor {
            flex-direction: row;
        }

        aside.aside {
            flex: 1;
        }

        article {
            flex: 3;
        }


        article {


            flex: 3; /* Toma 3 partes del espacio */
            background: var(--blanco);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        article h2 {
            color: var(--principal);
            margin-bottom: 15px;
        }

        footer {
            text-align: center;
            padding: 80px;
            background: var(--principal);
            color: white;
            margin-top: 80px;
        }

        /* Responsivo: Si la pantalla es pequeña, se pone uno bajo otro */
        @media (max-width: 768px) {
            .contenedor {
                flex-direction: column;
            }
            nav {
                min-height: auto;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Bienvenido al Consultorio Feliz</h1>
    <img src="dentistas.jpg" alt="Instalaciones del consultorio" width="100">
</header>

<div class="nav-horizontal" aria-label="Barra de navegación">
    <ul>
        <li><a href="index.html">Inicio</a></li>
        <li><a href="pacientes.html">Pacientes</a></li>
        <li><a href="dentistas.html">Dentista</a></li>
        <li><a href="citas.html">Citas</a></li>
    </ul>
</div>

<div class="contenedor">
    <aside class="aside">
        <h3>Nuestros Servicios</h3>
        <ul>
            <img src="paciente.jpg" alt="Instalaciones del consultorio" width="100">
        </ul>
    
    </aside>
    <article>
        <h2>Cuidamos tu bienestar</h2>
        <p>En el <strong>Consultorio Feliz</strong>, nuestra prioridad es brindarte una atención humana y profesional. Contamos con tecnología de punta y un equipo listo para atenderte y tener una sonrisa en esa cara amargada.</p>
        <br>
        <p>Estamos ubicados en el corazón de la ciudad en ciudad juarez, con horarios flexibles para que nunca descuides lo más importante: tu salud bocal.</p>
    </article>
    
</div>


<footer>
    <p>Cristian ariel garcia alvarez</p>
    <p>Implementa una base de datos no relacionales</p>
    <p>4J</p>
    <p>programacion</p>
    <img src="dentistas.jpg" alt="Instalaciones del consultorio" width="100">
</footer>



</body>
</html>
