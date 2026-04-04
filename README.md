<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ciencias Naturales - L.B. Simón Rodríguez</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        body { font-family: 'Poppins', sans-serif; scroll-behavior: smooth; }
        .hero-gradient { background: linear-gradient(135deg, #1e3a8a 0%, #10b981 100%); }
        .glass { background: rgba(255, 255, 255, 0.95); backdrop-filter: blur(10px); }
        .card-shadow { box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1); }
    </style>
</head>
<body class="bg-slate-50 text-gray-800">

    <nav class="glass shadow-sm sticky top-0 z-50 border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-4 h-16 flex justify-between items-center">
            <span class="text-2xl font-bold text-blue-700">Ciencias<span class="text-green-600 italic">Aricagua</span></span>
            <div class="flex items-center gap-4">
                <div id="adminBadge" class="hidden bg-green-100 text-green-700 text-[10px] px-2 py-1 rounded-full font-bold">MODO ADMIN</div>
                <button onclick="toggleAdminLogin()" class="text-xs bg-slate-800 text-white px-4 py-2 rounded-full hover:bg-slate-700 transition shadow-md">
                    <i class="fas fa-lock mr-2"></i> Admin
                </button>
            </div>
        </div>
    </nav>

    <header class="hero-gradient text-white py-20 px-4 text-center">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-4xl md:text-6xl font-extrabold mb-4 uppercase tracking-tighter">Liceo "Simón Rodríguez"</h1>
            <p class="text-xl mb-10 text-blue-50">Guía Interactiva de Ciencias Naturales - 3er Año</p>
            <div class="flex flex-wrap justify-center gap-4 bg-black/10 p-2 rounded-2xl w-fit mx-auto">
                <button onclick="switchTab('canaima')" id="btn-canaima" class="px-8 py-3 rounded-xl font-bold transition bg-white text-blue-700 shadow-lg">Canaima 🐧</button>
                <button onclick="switchTab('windows')" id="btn-windows" class="px-8 py-3 rounded-xl font-bold transition text-white opacity-70 hover:opacity-100">Windows 🪟</button>
            </div>
        </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 py-12">
        
        <section id="matematica" class="mb-16 bg-white p-8 rounded-[2rem] card-shadow border border-blue-100">
            <div class="flex items-center mb-8">
                <div class="w-12 h-12 bg-blue-600 text-white rounded-xl flex items-center justify-center mr-4 shadow-lg">
                    <i class="fas fa-calculator text-xl"></i>
                </div>
                <h2 class="text-3xl font-bold text-slate-800">Matemática: Ecuaciones Cuadráticas</h2>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="space-y-6">
                    <div class="bg-blue-50 p-6 rounded-2xl border-l-4 border-blue-600">
                        <h4 class="font-bold text-blue-800 mb-2">Explicación Paso a Paso</h4>
                        <p class="text-sm text-blue-700 leading-relaxed">
                            Para resolver $ax^2 + bx + c = 0$, usamos la <b>Fórmula General</b>. 
                            Primero identificamos los coeficientes, luego calculamos el <b>Discriminante</b> ($b^2 - 4ac$). Si es positivo, tenemos dos soluciones.
                        </p>
                        <div class="mt-4 p-3 bg-white rounded-lg text-center font-mono text-blue-900 border border-blue-200">
                            x = (-b ± √(b² - 4ac)) / 2a
                        </div>
                    </div>
                    <div class="p-6 border-2 border-dashed border-slate-200 rounded-2xl">
                        <h4 class="font-bold text-slate-700 mb-2">Ejercicio Resuelto</h4>
                        <p class="text-sm italic">Resolver: x² - 5x + 6 = 0</p>
                        <p class="text-xs mt-2 text-slate-500">
                            1. a=1, b=-5, c=6<br>
                            2. Disc: (-5)² - 4(1)(6) = 25 - 24 = 1<br>
                            3. x = (5 ± 1) / 2 <br>
                            <b>Resultados: x₁ = 3, x₂ = 2</b>
                        </p>
                    </div>
                </div>
                <div class="bg-slate-900 text-white p-8 rounded-3xl shadow-xl">
                    <h4 class="text-xl font-bold mb-4 text-blue-400"><i class="fas fa-edit mr-2"></i> Tarea para el Estudiante</h4>
                    <p class="text-sm mb-6 opacity-80">Copia esto en tu cuaderno y entrégalo al profesor:</p>
                    <div class="bg-white/10 p-6 rounded-xl border border-white/20">
                        <p class="font-bold text-lg mb-2">Problema: x² - 7x + 10 = 0</p>
                        <ul class="text-xs space-y-2 opacity-90">
                            <li>• Define los valores de a, b y c.</li>
                            <li>• Calcula el discriminante paso a paso.</li>
                            <li>• Encuentra las dos soluciones reales.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section id="fisica" class="mb-16 bg-white p-8 rounded-[2rem] card-shadow border border-green-100">
            <div class="flex items-center mb-8">
                <div class="w-12 h-12 bg-green-600 text-white rounded-xl flex items-center justify-center mr-4 shadow-lg">
                    <i class="fas fa-bolt text-xl"></i>
                </div>
                <h2 class="text-3xl font-bold text-slate-800">Física: Movimiento (MRU)</h2>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="space-y-6">
                    <div class="bg-green-50 p-6 rounded-2xl border-l-4 border-green-600">
                        <h4 class="font-bold text-green-800 mb-2">Explicación Paso a Paso</h4>
                        <p class="text-sm text-green-700 leading-relaxed">
                            En el <b>Movimiento Rectilíneo Uniforme</b>, la velocidad nunca cambia. La fórmula mágica es: <b>v = d / t</b> (Velocidad = Distancia entre Tiempo).
                        </p>
                        <div class="mt-4 p-3 bg-white rounded-lg text-center font-mono text-green-900 border border-green-200">
                            v = d / t | d = v · t | t = d / v
                        </div>
                    </div>
                    <div class="p-6 border-2 border-dashed border-slate-200 rounded-2xl">
                        <h4 class="font-bold text-slate-700 mb-2">Ejercicio Resuelto</h4>
                        <p class="text-sm italic">Un móvil recorre 200m en 40s. ¿Cuál es su v?</p>
                        <p class="text-xs mt-2 text-slate-500">
                            1. Datos: d=200m, t=40s<br>
                            2. v = 200 / 40<br>
                            <b>Resultado: v = 5 m/s</b>
                        </p>
                    </div>
                </div>
                <div class="bg-slate-900 text-white p-8 rounded-3xl shadow-xl">
                    <h4 class="text-xl font-bold mb-4 text-green-400"><i class="fas fa-flask mr-2"></i> Práctica Evaluable</h4>
                    <div class="bg-white/10 p-6 rounded-xl border border-white/20">
                        <p class="font-bold text-lg mb-2">Experimento en Casa:</p>
                        <p class="text-xs opacity-90 leading-relaxed">
                            Mide una distancia de 5 metros en el piso. Camina a paso normal y mide el tiempo con tu celular. Calcula tu velocidad y responde: ¿Qué pasaría con el tiempo si caminas más rápido? Justifica con la fórmula.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <section id="quimica" class="mb-16 bg-white p-8 rounded-[2rem] card-shadow border border-purple-100">
            <div class="flex items-center mb-8">
                <div class="w-12 h-12 bg-purple-600 text-white rounded-xl flex items-center justify-center mr-4 shadow-lg">
                    <i class="fas fa-vial text-xl"></i>
                </div>
                <h2 class="text-3xl font-bold text-slate-800">Química: El Átomo y la Tabla</h2>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="space-y-6">
                    <div class="bg-purple-50 p-6 rounded-2xl border-l-4 border-purple-600">
                        <h4 class="font-bold text-purple-800 mb-2">Explicación Paso a Paso</h4>
                        <p class="text-sm text-purple-700 leading-relaxed">
                            El <b>Número Atómico (Z)</b> nos dice cuántos protones tiene un átomo. El <b>Número Másico (A)</b> es la suma de protones y neutrones en el núcleo.
                        </p>
                    </div>
                    <div class="p-6 border-2 border-dashed border-slate-200 rounded-2xl">
                        <h4 class="font-bold text-slate-700 mb-2">Ejemplo de Análisis</h4>
                        <p class="text-sm italic">Átomo de Sodio (Na): Z=11, A=23</p>
                        <p class="text-xs mt-2 text-slate-500">
                            • Protones: 11<br>
                            • Electrones: 11<br>
                            • Neutrones: 23 - 11 = 12
                        </p>
                    </div>
                </div>
                <div class="bg-slate-900 text-white p-8 rounded-3xl shadow-xl">
                    <h4 class="text-xl font-bold mb-4 text-purple-400"><i class="fas fa-microscope mr-2"></i> Actividad de Investigación</h4>
                    <div class="bg-white/10 p-6 rounded-xl border border-white/20">
                        <p class="text-xs opacity-90 mb-4">Usa una tabla periódica para completar los datos de estos tres elementos:</p>
                        <ul class="text-sm font-bold space-y-2">
                            <li class="flex justify-between"><span>1. Oxígeno (O)</span> <span class="font-normal text-[10px]">Hallar Z, A y Neutrones</span></li>
                            <li class="flex justify-between"><span>2. Hierro (Fe)</span> <span class="font-normal text-[10px]">Hallar Z, A y Neutrones</span></li>
                            <li class="flex justify-between"><span>3. Calcio (Ca)</span> <span class="font-normal text-[10px]">Hallar Z, A y Neutrones</span></li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section class="max-w-5xl mx-auto px-4 mb-20">
            <div class="bg-slate-900 rounded-[3rem] p-10 shadow-2xl">
                <h3 class="text-2xl font-bold text-white mb-8 flex items-center">
                    <i class="fas fa-link mr-4 text-blue-400"></i> Repositorio de Recursos Compartidos
                </h3>
                <form id="submissionForm" class="grid sm:grid-cols-7 gap-4 mb-10">
                    <input type="text" id="progName" placeholder="Nombre del programa" required class="sm:col-span-3 p-4 rounded-2xl bg-slate-800 text-white border border-slate-700 outline-none focus:ring-2 focus:ring-blue-500">
                    <input type="url" id="progLink" placeholder="URL (Enlace)" required class="sm:col-span-3 p-4 rounded-2xl bg-slate-800 text-white border border-slate-700 outline-none focus:ring-2 focus:ring-blue-500">
                    <button type="submit" class="bg-blue-600 text-white rounded-2xl font-bold hover:bg-blue-500 transition shadow-lg flex items-center justify-center">
                        <i class="fas fa-plus"></i>
                    </button>
                </form>
                <div id="resourceContainer" class="grid grid-cols-1 sm:grid-cols-2 gap-4"></div>
            </div>
        </section>
    </main>

    <div id="loginModal" class="fixed inset-0 bg-slate-900/90 hidden backdrop-blur-sm flex items-center justify-center z-[100] p-4">
        <div class="bg-white rounded-[2rem] p-10 w-full max-w-sm">
            <h3 class="text-2xl font-bold text-center mb-6">Acceso Docente</h3>
            <input type="password" id="adminPass" placeholder="Clave de acceso" class="w-full p-4 bg-slate-100 rounded-2xl mb-6 border-2 border-transparent focus:border-blue-500 outline-none">
            <button onclick="login()" class="w-full bg-blue-600 text-white py-4 rounded-2xl font-bold shadow-lg hover:bg-blue-700 mb-4">Entrar</button>
            <button onclick="toggleAdminLogin()" class="w-full text-slate-400 text-xs font-bold uppercase">Cerrar</button>
        </div>
    </div>

    <footer class="bg-white border-t py-16 text-center">
        <p class="text-2xl font-black text-slate-800">Cova W. & Hernández Y.</p>
        <p class="text-blue-600 font-bold text-sm mb-4">TÉCNICO EN SISTEMAS - PROYECTO DE GRADO</p>
        <p class="text-slate-400 text-[10px] uppercase tracking-widest">Aricagua, Estado Bolívar • 2026</p>
    </footer>

    <script>
        let resources = JSON.parse(localStorage.getItem('aricagua_data')) || [];
        let isAdmin = false;
        const PASS = "aricagua2024";

        function switchTab(os) {
            const btnC = document.getElementById('btn-canaima');
            const btnW = document.getElementById('btn-windows');
            if(os === 'canaima') {
                btnC.className = "px-8 py-3 rounded-xl font-bold transition bg-white text-blue-700 shadow-lg";
                btnW.className = "px-8 py-3 rounded-xl font-bold transition text-white opacity-70";
            } else {
                btnW.className = "px-8 py-3 rounded-xl font-bold transition bg-white text-blue-700 shadow-lg";
                btnC.className = "px-8 py-3 rounded-xl font-bold transition text-white opacity-70";
            }
        }

        document.getElementById('submissionForm').onsubmit = (e) => {
            e.preventDefault();
            const res = { id: Date.now(), name: document.getElementById('progName').value, link: document.getElementById('progLink').value, status: 'Pendiente' };
            resources.unshift(res);
            save();
            e.target.reset();
        };

        function save() {
            localStorage.setItem('aricagua_data', JSON.stringify(resources));
            render();
        }

        function render() {
            const container = document.getElementById('resourceContainer');
            container.innerHTML = resources.length ? '' : '<p class="text-slate-500 text-center col-span-2">No hay enlaces compartidos.</p>';
            resources.forEach(r => {
                const div = document.createElement('div');
                div.className = "bg-slate-800/50 p-5 rounded-2xl flex justify-between items-center border border-slate-700/50";
                div.innerHTML = `
                    <div class="overflow-hidden">
                        <p class="font-bold text-blue-400 truncate text-sm">${r.name}</p>
                        <a href="${r.link}" target="_blank" class="text-[9px] text-slate-500 hover:text-white">Click para abrir link</a>
                    </div>
                    <div class="flex gap-2">
                        <span class="text-[8px] px-2 py-1 rounded-full font-bold ${r.status === 'Verificado' ? 'bg-green-500/20 text-green-400' : 'bg-orange-500/20 text-orange-400'}">${r.status}</span>
                        ${isAdmin ? `<button onclick="approve(${r.id})" class="text-green-400 text-xs"><i class="fas fa-check"></i></button>
                                     <button onclick="del(${r.id})" class="text-red-400 text-xs"><i class="fas fa-trash"></i></button>` : ''}
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function toggleAdminLogin() { document.getElementById('loginModal').classList.toggle('hidden'); }
        function login() {
            if(document.getElementById('adminPass').value === PASS) {
                isAdmin = true;
                document.getElementById('adminBadge').classList.remove('hidden');
                toggleAdminLogin();
                render();
            } else { alert("Clave incorrecta"); }
        }
        function approve(id) { resources = resources.map(r => r.id === id ? {...r, status: 'Verificado'} : r); save(); }
        function del(id) { if(confirm("¿Eliminar?")) { resources = resources.filter(r => r.id !== id); save(); } }

        render();
    </script>
</body>
</html>
