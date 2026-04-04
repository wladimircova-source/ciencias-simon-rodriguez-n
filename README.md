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
        .transition-all { transition: all 0.3s ease; }
    </style>
</head>
<body class="bg-slate-50 text-gray-800">

    <nav class="glass shadow-sm sticky top-0 z-50 border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-4 h-16 flex justify-between items-center">
            <span class="text-2xl font-bold text-blue-700 tracking-tight">Ciencias<span class="text-green-600 italic">Aricagua</span></span>
            <div class="flex items-center gap-4">
                <div id="adminBadge" class="hidden bg-green-100 text-green-700 text-[10px] px-2 py-1 rounded-full font-bold uppercase">Modo Admin</div>
                <button onclick="toggleAdminLogin()" class="text-xs bg-slate-800 text-white px-4 py-2 rounded-full hover:bg-slate-700 transition-all shadow-md">
                    <i class="fas fa-user-shield mr-2"></i> Acceso
                </button>
            </div>
        </div>
    </nav>

    <header class="hero-gradient text-white py-20 px-4 text-center shadow-inner">
        <div class="max-w-4xl mx-auto">
            <div class="inline-block bg-white/20 px-4 py-1 rounded-full text-xs font-semibold mb-4 backdrop-blur-md">PROMOCIÓN 2026</div>
            <h1 class="text-4xl md:text-6xl font-extrabold mb-4 tracking-tighter uppercase">Liceo "Simón Rodríguez"</h1>
            <p class="text-xl mb-10 text-blue-50 font-light max-w-2xl mx-auto">Plataforma interactiva para el fortalecimiento académico de 3er Año en Ciencias Naturales.</p>
            
            <div class="flex flex-wrap justify-center gap-4 bg-black/10 p-2 rounded-2xl w-fit mx-auto backdrop-blur-sm">
                <button onclick="switchTab('canaima')" id="btn-canaima" class="px-8 py-3 rounded-xl font-bold transition-all shadow-lg bg-white text-blue-700">Modo Canaima 🐧</button>
                <button onclick="switchTab('windows')" id="btn-windows" class="px-8 py-3 rounded-xl font-bold transition-all opacity-70 text-white hover:opacity-100">Modo Windows 🪟</button>
            </div>
        </div>
    </header>

    <section class="py-16 max-w-7xl mx-auto px-4 -mt-10">
        <div class="grid md:grid-cols-3 gap-8">
            <div class="bg-white p-8 rounded-3xl shadow-xl border border-gray-50 transform hover:-translate-y-2 transition-all">
                <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fas fa-calculator text-blue-600 text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Matemática</h3>
                <p class="text-gray-500 text-sm leading-relaxed mb-6">Dominio de ecuaciones de segundo grado y funciones reales.</p>
                <a href="#area-estudio" class="text-blue-600 font-bold text-sm hover:underline italic">Ver material educativo →</a>
            </div>
            
            <div class="bg-white p-8 rounded-3xl shadow-xl border border-gray-50 transform hover:-translate-y-2 transition-all">
                <div class="w-14 h-14 bg-green-100 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fas fa-atom text-green-600 text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Física</h3>
                <p class="text-gray-500 text-sm leading-relaxed mb-6">Estudio cinemático: Movimiento Rectilíneo Uniforme (MRU).</p>
                <a href="#area-estudio" class="text-green-600 font-bold text-sm hover:underline italic">Explorar guías →</a>
            </div>

            <div class="bg-white p-8 rounded-3xl shadow-xl border border-gray-50 transform hover:-translate-y-2 transition-all">
                <div class="w-14 h-14 bg-purple-100 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fas fa-vial text-purple-600 text-2xl"></i>
                </div>
                <h3 class="font-bold text-xl mb-3">Química</h3>
                <p class="text-gray-500 text-sm leading-relaxed mb-6">Propiedades de la materia y configuración electrónica.</p>
                <a href="#area-estudio" class="text-purple-600 font-bold text-sm hover:underline italic">Ver tabla periódica →</a>
            </div>
        </div>
    </section>

    <main class="max-w-7xl mx-auto px-4 pb-20">
        <div id="content-canaima" class="bg-blue-600 text-white p-8 rounded-3xl shadow-lg mb-12 flex flex-col md:flex-row items-center justify-between gap-6">
            <div>
                <h2 class="font-bold text-2xl mb-2 flex items-center"><i class="fab fa-linux mr-3"></i> Entorno Canaima GNU/Linux</h2>
                <p class="opacity-90">Optimiza tu aprendizaje con herramientas de Software Libre integradas.</p>
            </div>
            <div class="bg-black/20 p-4 rounded-xl font-mono text-xs border border-white/20 w-full md:w-auto">
                <span class="text-green-400">$</span> sudo apt install gnuplot geogebra
            </div>
        </div>

        <div id="content-windows" class="hidden bg-sky-500 text-white p-8 rounded-3xl shadow-lg mb-12 flex flex-col md:flex-row items-center justify-between gap-6">
            <div>
                <h2 class="font-bold text-2xl mb-2 flex items-center"><i class="fab fa-windows mr-3"></i> Entorno Windows</h2>
                <p class="opacity-90">Guía de instalación de aplicaciones educativas para PC convencionales.</p>
            </div>
            <div class="bg-white text-sky-600 px-6 py-2 rounded-lg font-bold text-sm">
                Instaladores .EXE
            </div>
        </div>

        <section id="area-estudio" class="bg-white p-10 rounded-[3rem] shadow-sm border border-gray-100">
            <h2 class="text-3xl font-black text-center mb-12 text-slate-800">Contenidos de 3er Año</h2>
            <div class="grid md:grid-cols-2 gap-10">
                <div class="group border-2 border-dashed border-slate-200 p-8 rounded-3xl hover:border-blue-400 transition-all">
                    <h4 class="font-bold text-blue-600 text-xl mb-4 flex items-center">
                        <span class="bg-blue-100 w-8 h-8 rounded-full flex items-center justify-center text-xs mr-3">01</span>
                        Matemática
                    </h4>
                    <div class="bg-slate-50 p-6 rounded-2xl mb-4">
                        <p class="text-center font-mono text-xl text-slate-700">ax² + bx + c = 0</p>
                    </div>
                    <p class="text-sm text-gray-500">Usa la fórmula general para hallar las raíces reales de la función.</p>
                </div>

                <div class="group border-2 border-dashed border-slate-200 p-8 rounded-3xl hover:border-green-400 transition-all">
                    <h4 class="font-bold text-green-600 text-xl mb-4 flex items-center">
                        <span class="bg-green-100 w-8 h-8 rounded-full flex items-center justify-center text-xs mr-3">02</span>
                        Física
                    </h4>
                    <div class="bg-slate-50 p-6 rounded-2xl mb-4">
                        <p class="text-center font-mono text-xl text-slate-700">v = Δx / Δt</p>
                    </div>
                    <p class="text-sm text-gray-500">Calcula el desplazamiento constante de un móvil en línea recta.</p>
                </div>
            </div>
        </section>
    </main>

    <section class="max-w-5xl mx-auto px-4 mb-20">
        <div class="bg-slate-900 rounded-[3rem] p-10 shadow-2xl relative overflow-hidden">
            <div class="absolute top-0 right-0 p-10 opacity-10">
                <i class="fas fa-link text-9xl text-white"></i>
            </div>
            <h3 class="text-2xl font-bold text-white mb-8 flex items-center">
                <i class="fas fa-share-nodes mr-4 text-blue-400"></i> Repositorio de Recursos
            </h3>
            <form id="submissionForm" class="grid sm:grid-cols-7 gap-4 mb-10 relative z-10">
                <input type="text" id="progName" placeholder="Nombre del programa" required class="sm:col-span-3 p-4 rounded-2xl bg-slate-800 text-white border border-slate-700 outline-none focus:ring-2 focus:ring-blue-500 transition-all">
                <input type="url" id="progLink" placeholder="Enlace de descarga" required class="sm:col-span-3 p-4 rounded-2xl bg-slate-800 text-white border border-slate-700 outline-none focus:ring-2 focus:ring-blue-500 transition-all">
                <button type="submit" class="bg-blue-600 text-white rounded-2xl font-bold hover:bg-blue-500 transition-all shadow-lg flex items-center justify-center">
                    <i class="fas fa-plus"></i>
                </button>
            </form>
            <div id="resourceContainer" class="grid grid-cols-1 sm:grid-cols-2 gap-4 max-h-[400px] overflow-y-auto custom-scrollbar">
                </div>
        </div>
    </section>

    <div id="loginModal" class="fixed inset-0 bg-slate-900/90 hidden backdrop-blur-sm flex items-center justify-center z-[100] p-4">
        <div class="bg-white rounded-[2rem] p-10 w-full max-w-sm shadow-2xl">
            <div class="text-center mb-8">
                <div class="w-20 h-20 bg-blue-50 rounded-full flex items-center justify-center mx-auto mb-4">
                    <i class="fas fa-unlock-alt text-3xl text-blue-600"></i>
                </div>
                <h3 class="text-2xl font-bold">Panel de Control</h3>
                <p class="text-gray-400 text-sm mt-2">Solo personal autorizado</p>
            </div>
            <input type="password" id="adminPass" placeholder="Introducir clave" class="w-full p-4 bg-slate-100 rounded-2xl mb-6 border-2 border-transparent focus:border-blue-500 outline-none transition-all">
            <button onclick="login()" class="w-full bg-blue-600 text-white py-4 rounded-2xl font-bold shadow-lg hover:bg-blue-700 transition-all mb-4">Validar Credenciales</button>
            <button onclick="toggleAdminLogin()" class="w-full text-slate-400 text-sm font-semibold uppercase tracking-widest">Cancelar</button>
        </div>
    </div>

    <footer class="bg-white border-t border-gray-100 py-16 text-center">
        <div class="max-w-7xl mx-auto px-4">
            <p class="text-2xl font-black text-slate-800 mb-2">Cova W. & Hernández Y.</p>
            <p class="text-blue-600 font-bold mb-6 text-sm">PROYECTO DE GRADO - TÉCNICO EN SISTEMAS</p>
            <div class="flex justify-center gap-6 text-slate-300 text-xl mb-10">
                <i class="fab fa-github hover:text-slate-900 cursor-pointer"></i>
                <i class="fab fa-linkedin hover:text-slate-900 cursor-pointer"></i>
            </div>
            <p class="text-slate-400 text-[10px] uppercase tracking-[0.5em]">L.B. Simón Rodríguez • Aricagua 2026</p>
        </div>
    </footer>

    <script>
        // Cargar recursos guardados al iniciar
        let resources = JSON.parse(localStorage.getItem('aricagua_resources')) || [];
        let isAdmin = false;
        const MASTER_PASS = "aricagua2024";

        function switchTab(os) {
            const canaima = document.getElementById('content-canaima');
            const windows = document.getElementById('content-windows');
            const btnC = document.getElementById('btn-canaima');
            const btnW = document.getElementById('btn-windows');

            if(os === 'canaima') {
                canaima.classList.remove('hidden'); windows.classList.add('hidden');
                btnC.className = "px-8 py-3 rounded-xl font-bold transition-all shadow-lg bg-white text-blue-700";
                btnW.className = "px-8 py-3 rounded-xl font-bold transition-all opacity-70 text-white hover:opacity-100";
            } else {
                windows.classList.remove('hidden'); canaima.classList.add('hidden');
                btnW.className = "px-8 py-3 rounded-xl font-bold transition-all shadow-lg bg-white text-blue-700";
                btnC.className = "px-8 py-3 rounded-xl font-bold transition-all opacity-70 text-white hover:opacity-100";
            }
        }

        document.getElementById('submissionForm').onsubmit = (e) => {
            e.preventDefault();
            const newRes = {
                id: Date.now(),
                name: document.getElementById('progName').value,
                link: document.getElementById('progLink').value,
                status: 'Pendiente'
            };
            resources.unshift(newRes);
            saveAndRender();
            e.target.reset();
        };

        function saveAndRender() {
            localStorage.setItem('aricagua_resources', JSON.stringify(resources));
            renderResources();
        }

        function renderResources() {
            const container = document.getElementById('resourceContainer');
            container.innerHTML = '';
            
            if (resources.length === 0) {
                container.innerHTML = '<p class="text-slate-500 text-sm italic col-span-2 text-center py-10">No hay enlaces compartidos aún.</p>';
                return;
            }

            resources.forEach(res => {
                const div = document.createElement('div');
                div.className = "bg-slate-800/50 p-5 rounded-2xl flex justify-between items-center border border-slate-700/50 hover:bg-slate-800 transition-all";
                div.innerHTML = `
                    <div class="overflow-hidden mr-4">
                        <p class="font-bold text-blue-400 truncate">${res.name}</p>
                        <a href="${res.link}" target="_blank" class="text-[10px] text-slate-500 hover:text-blue-300 transition-all truncate block">Abrir enlace externo</a>
                    </div>
                    <div class="flex items-center gap-3">
                        <span class="text-[9px] px-2 py-1 rounded-full font-bold ${res.status === 'Verificado' ? 'bg-green-500/20 text-green-400' : 'bg-orange-500/20 text-orange-400'}">${res.status}</span>
                        ${isAdmin ? `
                            <button onclick="approve(${res.id})" class="text-green-400 hover:scale-110 transition-all"><i class="fas fa-check-circle"></i></button>
                            <button onclick="deleteRes(${res.id})" class="text-red-400 hover:scale-110 transition-all"><i class="fas fa-trash"></i></button>
                        ` : ''}
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function toggleAdminLogin() { document.getElementById('loginModal').classList.toggle('hidden'); }

        function login() {
            if(document.getElementById('adminPass').value === MASTER_PASS) {
                isAdmin = true;
                document.getElementById('adminBadge').classList.remove('hidden');
                toggleAdminLogin();
                renderResources();
            } else { alert("❌ Clave incorrecta"); }
        }

        function approve(id) {
            resources = resources.map(r => r.id === id ? {...r, status: 'Verificado'} : r);
            saveAndRender();
        }

        function deleteRes(id) {
            if(confirm("¿Estás seguro de eliminar este recurso?")) {
                resources = resources.filter(r => r.id !== id);
                saveAndRender();
            }
        }

        // Render inicial
        renderResources();
    </script>
</body>
</html>
