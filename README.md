# LaPalomaSeafoodWeb
Pagina web de Mariscos
    [Uploading index.html…]<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Restaurante especializado en mariscos frescos en Altata, Navolato. Disfruta de los mejores platillos del mar en un ambiente único.">
    <title>La Paloma Seafood - Marisquería Premium en Altata</title>
    
    <!-- Estilos externos -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/css/lightbox.min.css">

    <style>
        :root {
            --primary-color: #0a3d62;
            --secondary-color: #e55039;
        }

        .hero {
            /* Fondo corregido (debes poner la imagen en la carpeta 'imagen/') */
            background: linear-gradient(rgba(10, 61, 98, 0.8), rgba(10, 61, 98, 0.8)), 
                        url('imagenes/Logo.jpg') center/cover no-repeat;
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
        }

        .section-title {
            color: var(--primary-color);
            position: relative;
            margin-bottom: 3rem;
        }

        .section-title:after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: var(--secondary-color);
        }

        .menu-card {
            transition: transform 0.3s;
            border: none;
            border-radius: 15px;
            overflow: hidden;
        }

        .menu-card:hover {
            transform: translateY(-10px);
        }

        .btn-primary {
            background: var(--secondary-color);
            border: none;
            padding: 12px 30px;
            transition: all 0.3s;
        }

        .btn-primary:hover {
            background: #b71540;
            transform: scale(1.05);
        }

        .contact-info-box {
            background: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            padding: 2rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .social-icon {
            font-size: 1.8rem;
            margin: 0 10px;
            color: var(--primary-color);
            transition: color 0.3s;
        }

        .social-icon:hover {
            color: var(--secondary-color);
        }

        .map-container {
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
        }

        .gallery-item img {
            transition: transform 0.3s;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }
    </style>
</head>

<body>
    <!-- Header -->
    <header class="hero text-blue text-center">
        <div class="container">
            <div class="contact-info-box">
                <img src="imagenes/Logo.png" alt="Logo La Paloma Seafood" class="mb-4" style="max-width: 200px;">
                <h1 class="display-4 mb-4">La Paloma Seafood</h1>
                <div class="lead mb-4">
                    <p class="mb-3">
                        <i class="fas fa-phone-alt mr-2"></i>
                        <a href="tel:6721149594" class="text-dark">672 114 9594</a>
                    <p class="mb-3">
                        <i class="fas fa-map-marker-alt mr-2"></i>
                        Muelle 33 Local 28, Altata, Navolato Sinaloa
                    </p>
                    <p class="mb-0">
                        <i class="fas fa-clock mr-2"></i>
                        Horario: Lunes a Domingo 9:00 AM - 10:00 PM
                    </p>
                </div>
                <div class="mt-4">
                    <a href="#menu" class="btn btn-primary mr-3">Ver Menú</a>
                    <a href="#contacto" class="btn btn-outline-dark">Cómo llegar</a>
                </div>
                <div class="mt-4">
                    <a href="#" class="social-icon"><i class="fab fa-facebook"></i></a>
                    <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="social-icon"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
        </div>
    </header>

    <!-- Menú -->
    <section id="menu" class="py-5 bg-light">
        <div class="container">
            <h2 class="section-title text-center">Nuestros Especiales</h2>
            <div class="row">
                <div class="col-md-4 mb-4">
                    <div class="menu-card">
                        <img src="imagenes/tosCam.jpg" class="card-img-top" alt="Tostadas de Camarón">
                        <div class="card-body text-center">
                            <h5 class="card-title">Tostadas de Camarón</h5>
                            <p class="text-muted">Frescos camarones del día con nuestra salsa especial</p>
                            <p class="h5 text-primary">$120 MXN</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-4 mb-4">
                    <div class="menu-card">
                        <img src="imagenes/TosAtun.jpg" class="card-img-top" alt="Tostadas de Atún">
                        <div class="card-body text-center">
                            <h5 class="card-title">Tostadas de Atún</h5>
                            <p class="text-muted">Atún fresco marinado con especias</p>
                            <p class="h5 text-primary">$150 MXN</p>
                        </div>
                    </div>
                </div>

                <div class="col-md-4 mb-4">
                    <div class="menu-card">
                        <img src="imagenes/Botana.jpg" class="card-img-top" alt="Camarones al Coco">
                        <div class="card-body text-center">
                            <h5 class="card-title">Botana </h5>
                            <p class="text-muted">deliciosa botana de Cam mix Pulpo Callo Y mango </p>
                            <p class="h5 text-primary">$400 MXN</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-4">
                <a href="imagenes/MenuPdf.pdf" class="btn btn-primary" download>
                    <i class="fas fa-download mr-2"></i>Descargar Menú Completo
                </a>
            </div>
        </div>
    </section>

    <!-- Galería -->
    <!-- Sección de Galería con Carrusel Automático -->
<section class="py-5">
    <div class="container">
        <h2 class="section-title text-center">Nuestros Platillos</h2>
        <div class="row">
            <div class="col-md-8 mx-auto">
                <div id="foodCarousel" class="carousel slide" data-ride="carousel">
                    <!-- Indicadores -->
                    <ol class="carousel-indicators">
                        <li data-target="#foodCarousel" data-slide-to="0" class="active"></li>
                        <li data-target="#foodCarousel" data-slide-to="1"></li>
                        <li data-target="#foodCarousel" data-slide-to="2"></li>
                    </ol>
                    
                    <!-- Slides -->
                    <div class="carousel-inner rounded-lg">
                        <div class="carousel-item active">
                            <img src="imagenes/Atarralla.jpg" class="d-block w-100" alt="Tostadas de Camarón">
                            <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
                                <h5>Atarralla</h5>
                                <p>filete zarandeado Servido con cama de sal seca prendido en fuego</p>
                            </div>
                        </div>
                        <div class="carousel-item">
                            <img src="imagenes/BotanaCamaron.jpg" class="d-block w-100" alt="Tostadas de Atún">
                            <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
                                <h5>Botana </h5>
                                <p>Camaron Y Pulpo</p>
                            </div>
                        </div>
                        <div class="carousel-item">
                            <img src="imagenes/Curricanes.jpg" class="d-block w-100" alt="Curricanes">
                            <div class="carousel-caption d-none d-md-block bg-dark bg-opacity-50 rounded">
                                <h5>Curricanes </h5>
                                <p>deliciosa entrada de curricanes</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Controles -->
                    <a class="carousel-control-prev" href="#foodCarousel" role="button" data-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="sr-only">Anterior</span>
                    </a>
                    <a class="carousel-control-next" href="#foodCarousel" role="button" data-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="sr-only">Siguiente</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</section>

<style>
    /* Estilos para el carrusel */
    .carousel {
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        border-radius: 15px;
        overflow: hidden;
    }
    .carousel-item {
        transition: transform 0.6s ease;
    }
    .carousel-item img {
        max-height: 500px;
        object-fit: cover;
    }
    .carousel-indicators li {
        width: 12px;
        height: 12px;
        border-radius: 50%;
        background-color: #0a3d62;
    }
    .carousel-control-prev-icon,
    .carousel-control-next-icon {
        background-color: #e55039;
        border-radius: 50%;
        padding: 20px;
        background-size: 60%;
    }
    .carousel-caption {
        right: 15%;
        left: 15%;
        padding-bottom: 30px;
    }
</style>

<script>
    // Configuración del carrusel automático
    document.addEventListener('DOMContentLoaded', function() {
        var myCarousel = document.querySelector('#foodCarousel');
        var carousel = new bootstrap.Carousel(myCarousel, {
            interval: 5000,
            wrap: true
        });
        
        // Pausa al hacer hover
        myCarousel.addEventListener('mouseenter', function() {
            carousel.pause();
        });
        myCarousel.addEventListener('mouseleave', function() {
            carousel.cycle();
        });
    });
</script>
    <!-- Mapa -->
    <section id="contacto" class="py-5 bg-light">
        <div class="container">
            <h2 class="section-title text-center">Cómo Llegar</h2>
            <div class="map-container">
                <iframe src="https://maps.app.goo.gl/fR9YV7sVxEccAwug9" 
                        width="100%" 
                        height="450" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <div class="mt-4">
        <!-- Enlace de Facebook corregido -->
        <a href="https://www.facebook.com/share/1BAxkcmHhd/" 
           class="social-icon"
           target="_blank"
           rel="noopener noreferrer">
            <i class="fab fa-facebook"></i>
        </a>
        <a href="#" class="social-icon"><i class="https://www.instagram.com/la_paloma_sea_food?igsh=MXM2aXI2M2hoZXpoNw=="></i></a>
        <a href="#" class="social-icon"><i class="fab fa-whatsapp"></i></a>
    </div>

    <!-- Scripts -->
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/js/lightbox.min.js"></script>
    <script>
        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
()
