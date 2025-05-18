<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ikea - Muebles y Decoración</title>
    <style>
        /* Estilos Base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        body {
            background-color: #f5f5f5;
            color: #333;
        }

        .contenedor {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Encabezado */
        .encabezado {
            background: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .barra-navegacion {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #faf203;
        }

        .menu {
            display: flex;
            gap: 2rem;
        }

        .menu a {
            text-decoration: none;
            color: #444;
            font-weight: 500;
            transition: color 0.3s;
        }

        .menu a:hover {
            color: #0077B6;
        }

        .carrito {
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Banner Principal */
        .banner {
            height: 70vh;
            background: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.1)),
                        url('sala-moderna.jpg') center/cover;
            margin-bottom: 3rem;
            display: flex;
            align-items: center;
        }

        .texto-banner {
            color: white;
            max-width: 600px;
            padding: 2rem;
        }

        .texto-banner h1 {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        /* Productos Destacados */
        .seccion-titulo {
            margin: 3rem 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .grid-productos {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .tarjeta-producto {
            background: white;
            border-radius: 8px;
            padding: 1rem;
            transition: transform 0.3s;
        }

        .tarjeta-producto:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .imagen-producto {
            height: 200px;
            background: #f1f3f5;
            border-radius: 4px;
            margin-bottom: 1rem;
        }

        .precio {
            color: #0077B6;
            font-weight: bold;
            margin: 0.5rem 0;
        }

        .boton {
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-weight: 500;
        }

        .boton-primario {
            background: #0077B6;
            color: white;
        }

        /* Ofertas */
        .etiqueta-oferta {
            background: #e63946;
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
            position: absolute;
            top: 1rem;
            right: 1rem;
        }

        .precio-original {
            text-decoration: line-through;
            color: #999;
            margin-right: 0.5rem;
        }

        /* Pie de página */
        .pie-pagina {
            background: #2d3436;
            color: white;
            padding: 4rem 0 2rem;
            margin-top: 4rem;
        }

        .grid-pie {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .enlaces-pie a {
            color: #ccc;
            text-decoration: none;
            display: block;
            margin-bottom: 0.5rem;
        }

        .redes-sociales {
            display: flex;
            gap: 1rem;
            font-size: 1.5rem;
        }

        .legal {
            border-top: 1px solid #444;
            padding-top: 2rem;
            text-align: center;
        }
    </style>
</head>
<body>
    <header class="encabezado">
        <nav class="contenedor barra-navegacion">
            <div class="logo">Ikea</div>
            <div class="menu">
                <a href="#">Categorías</a>
                <a href="#">Novedades</a>
                <a href="#">Ofertas</a>
                <a href="#">Inspiración</a>
                <a href="#">Servicios</a>
            </div>
            <div class="carrito">🛒</div>
        </nav>
    </header>

    <section class="banner">
        <div class="contenedor">
            <div class="texto-banner">
                <h1>Transforma tu hogar con estilo y funcionalidad</h1>
                <button class="boton boton-primario">Ver colección</button>
            </div>
        </div>
    </section>

    <main class="contenedor">
        <section class="productos-destacados">
            <div class="seccion-titulo">
                <h2>Productos Destacados</h2>
                <button class="boton boton-primario">Ver todos</button>
            </div>
            <div class="grid-productos">
                <div class="tarjeta-producto">
                    <div class="imagen-producto"></div>
                    <h3>Giromundi</h3>
                    <p class="precio">€599.00</p>
                    <button class="boton boton-primario">Ver más</button>
                </div>
                <!-- Repetir tarjetas de productos -->
            </div>
        </section>

        <section class="ofertas">
            <div class="seccion-titulo">
                <h2>Ofertas Limitadas</h2>
                <div class="contador">48:00:00 Restantes</div>
            </div>
            <div class="grid-productos">
                <div class="tarjeta-producto">
                    <div class="etiqueta-oferta">-30%</div>
                    <div class="imagen-producto"></div>
                    <h3>Mesa de Centro Nórdica</h3>
                    <p>
                        <span class="precio-original">€299.00</span>
                        <span class="precio">€209.30</span>
                    </p>
                    <button class="boton boton-primario">Comprar ahora</button>
                </div>
                <!-- Repetir tarjetas de ofertas -->
            </div>
        </section>
    </main>

    <footer class="pie-pagina">
        <div class="contenedor">
            <div class="grid-pie">
                <div>
                    <h4>Atención al Cliente</h4>
                    <div class="enlaces-pie">
                        <a href="#">Contacto</a>
                        <a href="#">Envíos</a>
                        <a href="#">Devoluciones</a>
                        <a href="#">Preguntas Frecuentes</a>
                    </div>
                </div>
                <div>
                    <h4>Tienda Física</h4>
                    <div class="enlaces-pie">
                        <a href="#">Localizador</a>
                        <a href="#">Horarios</a>
                        <a href="#">Eventos</a>
                    </div>
                </div>
                <div>
                    <h4>Redes Sociales</h4>
                    <div class="redes-sociales">
                        <a href="#">📘</a>
                        <a href="#">📸</a>
                        <a href="#">📌</a>
                    </div>
                </div>
            </div>
            <div class="legal">
                <p>© 2024 HogarModerno. Todos los derechos reservados</p>
                <div class="enlaces-pie">
                    <a href="#">Política de Privacidad</a>
                    <a href="#">Términos de Servicio</a>
                </div>
            </div>
        </div>
    </footer>
</body>
</html>
