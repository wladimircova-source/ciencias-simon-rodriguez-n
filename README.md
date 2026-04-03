
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Ciencias Naturales - Aricagua</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        .hero-gradient {
            background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);
        }

        .card-hover:hover {
            transform: translateY(-5px);
            transition: all 0.3s ease;
        }

        .science-bg {
            background-color: #f8fafc;
            background-image: url("https://www.transparenttextures.com/patterns/cubes.png");
        }
    </style>
</head>
<body class="science-bg text-gray-800">

    <!-- Navegación -->
    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex items-center">
                    <span class="text-2xl font-bold text-blue-700">Ciencias<span class="text-green-600 text-sm italic ml-1">Aricagua</span></span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#inicio" class="text-gray-600 hover:text-blue-700 font-medium">Inicio</a>
                    <a href="#materias" class="text-gray-600 hover:text-blue-700 font-medium">Materias</a>
                    <a href="#recursos" class="text-gray-600 hover:text-blue-700 font-medium">Recursos</a>
                    <a href="#contacto" class="bg-blue-600 text-white px-4 py-2 rounded-lg hover:bg-blue-700 transition">Contacto</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="inicio" class="hero-gradient text-white py-20 px-4 text-center">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">¡Bienvenidos, Estudiantes del Liceo Simón Rodríguez!</h1>
            <p class="text-xl mb-8 text-blue-100">Explora el fascinante mundo de la Matemática, Física y Química de forma divertida y digital en Aricagua.</p>
            <a href="#materias" class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-8 rounded-full text-lg transition-all shadow-lg">
                Comenzar a Aprender
            </a>
        </div>
    </header>

    <!-- Sección de Materias -->
    <section id="materias" class="py-16 max-w-7xl mx-auto px-4">
        <div class="text-center mb-12">
            <h2 class="text-3xl font-bold text-gray-900">Nuestras Áreas de Estudio</h2>
            <p class="text-gray-600 mt-2">Contenido diseñado especialmente para 3er Año</p>
        </div>

        <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100 card-hover text-center">
    <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-6">
        <i class="fas fa-calculator text-blue-600 text-2xl"></i>
    </div>
    <h3 class="text-xl font-bold mb-3">Matemática</h3>
    <p class="text-gray-600 mb-4 text-sm">Ecuaciones, funciones y geometría explicada con ejemplos de nuestra comunidad.</p>
    <a href="#seccion-ciencias" class="text-blue-600 font-semibold hover:underline cursor-pointer">Ver lecciones ↓</a>
</div>

<div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100 card-hover text-center">
    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-6">
        <i class="fas fa-atom text-green-600 text-2xl"></i>
    </div>
    <h3 class="text-xl font-bold mb-3">Física</h3>
    <p class="text-gray-600 mb-4 text-sm">Entiende el movimiento y la energía a través de simulaciones virtuales interactivas.</p>
    <a href="#seccion-ciencias" class="text-green-600 font-semibold hover:underline cursor-pointer">Explorar experimentos ↓</a>
</div>

<div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100 card-hover text-center">
    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-6">
        <i class="fas fa-vial text-purple-600 text-2xl"></i>
    </div>
    <h3 class="text-xl font-bold mb-3">Química</h3>
    <p class="text-gray-600 mb-4 text-sm">Desde la tabla periódica hasta las reacciones químicas que vemos en el día a día.</p>
    <a href="#seccion-ciencias" class="text-purple-600 font-semibold hover:underline cursor-pointer">Ver reacciones ↓</a>
</div>
    <!-- Interactivo: Reto Científico -->
    <section id="recursos" class="bg-blue-900 py-16 text-white px-4">
        <div class="max-w-4xl mx-auto">
            <div class="bg-white text-gray-800 p-8 rounded-3xl shadow-2xl">
                <h2 class="text-2xl font-bold mb-6 flex items-center">
                    <i class="fas fa-lightbulb text-yellow-500 mr-3"></i>
                    Reto Científico del Día
                </h2>
                <div id="quiz-container">
                    <p class="text-lg mb-6" id="question">¿Cuál es el símbolo químico del Oro, mineral que encontramos en nuestra región?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <button onclick="checkAnswer('Ag')" class="option-btn border-2 border-blue-100 p-4 rounded-xl hover:bg-blue-50 transition text-left">A) Ag</button>
                        <button onclick="checkAnswer('Au')" class="option-btn border-2 border-blue-100 p-4 rounded-xl hover:bg-blue-50 transition text-left">B) Au</button>
                        <button onclick="checkAnswer('Fe')" class="option-btn border-2 border-blue-100 p-4 rounded-xl hover:bg-blue-50 transition text-left">C) Fe</button>
                        <button onclick="checkAnswer('O')" class="option-btn border-2 border-blue-100 p-4 rounded-xl hover:bg-blue-50 transition text-left">D) O</button>
                    </div>
                    <div id="feedback" class="mt-6 hidden p-4 rounded-lg"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pie de Página -->
    <footer id="contacto" class="bg-white border-t border-gray-200 py-12">
        <div class="max-w-7xl mx-auto px-4 text-center">
            <h2 class="text-xl font-bold text-blue-700 mb-4">Proyecto Socio-Tecnológico</h2>
            <p class="text-gray-500">Realizado por: Cova W. & Hernández Y.</p>
            <p class="text-gray-500">Tutor: Henlys Velázquez</p>
            <p class="text-gray-400 text-sm mt-8">© 2026 Aricagua, Municipio Montes, Edo. Sucre. Todos los derechos reservados.</p>
        </div>
    </footer>

    <script>
        function checkAnswer(answer) {
            const feedback = document.getElementById('feedback');
            feedback.classList.remove('hidden', 'bg-green-100', 'bg-red-100', 'text-green-700', 'text-red-700');
            
            if (answer === 'Au') {
                feedback.innerHTML = "<strong>¡Correcto!</strong> El símbolo del Oro es Au (del latín Aurum). ¡Eres un genio químico!";
                feedback.classList.add('bg-green-100', 'text-green-700');
            } else {
                feedback.innerHTML = "<strong>Casi...</strong> Inténtalo de nuevo. Recuerda revisar la tabla periódica en la sección de Química.";
                feedback.classList.add('bg-red-100', 'text-red-700');
            }
        }

        // Simulación de carga para efectos visuales
        window.onload = () => {
            console.log("Blog Educativo Aricagua listo.");
        };
    </script>
</body>
</html>
