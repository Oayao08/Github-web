<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog - ZARIO</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Kaushan+Script&family=Gruppo&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: black;
            color: white;
            font-family: ' Gruppo ' ,sans-serif;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background-color: #222;
        }

        .logo-container {
            display: flex;
            align-items: center;
        }

        .logo-container img {
            height: 50px;
            margin-right: 15px;
        }

        .logo-text {
            font-family: 'Kaushan Script', cursive;
            font-size: 2rem;
            font-weight: bold;
            color: #fff;
            white-space: nowrap;
        }

        .logo-container a {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
        }

        nav {
            display: flex;
            gap: 20px;
        }

        nav a {
            font-family: 'Gruppo', sans-serif;
            color: #fff;
            text-decoration: none;
            font-size: 1.2rem;
            padding: 10px;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.2s;
        }

        /* Animación al pasar el mouse por encima */
        nav a:hover {
            background-color: #e4e4e4;
            color: #111;
        }

        /* Animación al hacer clic en el botón */
        nav a:active {
            transform: scale(0.95); /* Reduce el tamaño del botón */
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.5); /* Resplandor */
        }

        h1 {
            margin: 0;
            font-size: 2.5em;
            animation: fadeIn 1.5s ease-in-out;
        }

        .blog-container {
            width: 80%;
            margin: auto;
            padding: 40px 0;
        }

        .blog-section {
            margin-bottom: 60px;
        }

        .blog-section h2 {
            color: white;
            font-size: 2em;
            text-align: center;
            margin-bottom: 20px;
            animation: slideUp 1s ease-in-out;
        }

        .blog-post, .historia, .comparativa div, .motivacion {
            background-color: white;
            color: black;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0px 6px 15px rgba(255, 255, 255, 0.6);
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 1s ease-in-out forwards;
        }

        .blog-post {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        .blog-post img, .historia img {
            width: 40%;
            border-radius: 8px;
        }

        .blog-post div, .historia div {
            width: 60%;
        }

        .comparativa {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }

        .comparativa div {
            width: 45%;
            text-align: center;
        }

        .comparativa img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 8px;
        }

        .historia {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .historia img {
            width: 50%;
        }

        .motivacion {
            text-align: center;
            padding: 30px;
            margin-top: 50px;
        }

        .motivacion img {
            width: 100%;
            max-width: 600px;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        footer {
            text-align: center;
            padding: 40px;
            background-color: #222;
            margin-top: 40px;
            position: relative;
            overflow: hidden;
        }

        footer h2 {
            color: white;
            font-size: 1.8em;
            margin-bottom: 20px;
            animation: fadeInUp 1s ease-in-out;
        }

        footer .motivational-container img {
            width: 100%;
            object-fit: cover;
            opacity: 0.8;
        }

        footer .quote {
            color: white;
            font-size: 1.5em;
            font-weight: bold;
            position: absolute;
            top: 30%;
            left: 50%;
            transform: translateX(-50%);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
            animation: fadeInQuote 3s ease-in-out infinite;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        @keyframes slideImage {
            0% { transform: translateX(0); }
            100% { transform: translateX(-100%); }
        }

        @keyframes fadeInQuote {
            0% { opacity: 0; }
            50% { opacity: 1; }
            100% { opacity: 0; }
        }

        
    </style>
</head>
<body>

    <header>
        <div class="logo-container">
            <a href="home.html">
                <img src="logo.png" alt="Zario Logo">
                <div class="logo-text">Zario</div>
            </a>
        </div>
        <nav>
            <a href="tienda.html">Tienda</a>
            <a href="blog.html">Blog</a>
            <a href="tecnologia.html">Tecnología</a>
            <a href="contactos.html">Contacto</a>
        </nav>
    </header>


    <div class="blog-container">

        <!-- Sección de Reseñas -->
        <section class="blog-section">
            <h2>Reseñas de Automóviles</h2>
            <div class="blog-post">
                <img src="https://cdn.pixabay.com/photo/2017/09/20/16/41/pagani-2769165_1280.jpg" alt="Zario R6 GT">
                <div>
                    <h3>Zario R6 GT</h3>
                    <p>El Zario R6 GT es un deportivo de alto rendimiento que combina tecnología de vanguardia con una experiencia de conducción única. Su diseño aerodinámico y agresivo no solo resalta su carácter deportivo, sino que también optimiza la eficiencia y estabilidad a altas velocidades.</p>
                </div>
            </div>
            <!-- Nuevo cuadro de reseña añadido -->
            <div class="blog-post">
                <img src="https://www.exoticcarlist.com/blog/wp-content/uploads/2025/02/Koenigsegg-Agera.jpg" alt="Zario Serie 3 M2">
                <div>
                    <h3>Zario Serie 3 M2</h3>
                    <p>El Zario Serie 3 M2 es el futuro de la velocidad, un vehículo que fusiona innovación, potencia y precisión en un solo paquete. Diseñado para los entusiastas de la conducción deportiva, este modelo destaca por su aerodinámica optimizada y su avanzado tren motriz.</p>
                </div>
            </div>
        </section>

        <!-- Sección de Comparativas -->
        <section class="blog-section">
            <h2>Comparativa de Modelos</h2>
            <div class="comparativa">
                <div>
                    <h3>Zario Serie 3 M2</h3>
                    <img src="https://cdn.pixabay.com/photo/2014/09/07/22/32/koenigsegg-438460_1280.jpg" alt="Zario R6">
                    <p>Un análisis detallado entre los modelos Zario R6 y Zario R7 para ayudarte a elegir el mejor vehículo para ti.</p>
                </div>
                <div>
                    <h3>Zario R6 GT</h3>
                    <img src="https://cdn.pixabay.com/photo/2024/02/14/07/11/sports-car-8572636_960_720.png" alt="Zario R6 GT">
                    <p>Compara el rendimiento y las características clave de los Zario R8 y R6 para una elección informada.</p>
                </div>
            </div>
        </section>

    </div>

            <!-- Sección de Historia -->
            <section class="blog-section">
                <h2>Historia del Zario</h2> 
                <div class="historia">
                    <img src="https://cdn.pixabay.com/photo/2024/03/11/07/18/ai-generated-8626003_960_720.png" alt="Historia Zario">
                    <div>
                        <h3>Un legado de innovación</h3>
                        <p>La marca Zario està destinada a revolucionar el món de l'automòbil amb els seus dissenys audaces i el seu ferm compromís amb la sostenibilitat. Fundada amb la visió de transformar la mobilitat, Zario aposta per tecnologies innovadores i materials ecològics per reduir l'impacte ambiental. Cada vehicle és dissenyat per oferir eficiència, estil i respecte pel planeta, marcant el camí cap a un futur més sostenible a les carreteres.</p>
                    </div>
                </div>
            </section>

<!-- Nuevo pie de página -->
<footer>
    <div class="motivational-container">
        <div class="gif-background">
            <img src="https://cdn.pixabay.com/photo/2015/07/27/22/52/road-863661_1280.jpg" alt="Motivational">
        </div>
    </div>
    <!-- Frase motivacional centrada -->
    <div class="quote">"El único modo de hacer un gran trabajo es amar lo que haces." - Steve Jobs</div>
</footer>
</body>




</html>
