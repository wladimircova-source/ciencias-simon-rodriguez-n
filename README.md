
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
        .hero-gradient { background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%); }
        .tab-active { border-bottom: 4px solid #1e40af; color: #1e40af; font-weight: bold; }
    </style>
</head>
<body class="bg-slate-50 text-gray-800">

    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 h-16 flex justify-between items-center">
            <span class="text-xl font-bold text-blue-700">Ciencias<span class="text-green-600 italic ml-1">Aricagua</span></span>
            <div class="flex gap-4">
                <button onclick="toggleAdminLogin()" class="text-xs bg-slate-800 text-white px-3 py-2 rounded-lg hover:bg-slate-700 transition">
                    <i class="fas fa-lock mr-1"></i> Admin
                </button>
            </div>
        </div>
    </nav>

    <header class="hero-gradient text-white py-16 px-4 text-center">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-3xl md:text-5xl font-bold mb-4 uppercase">Liceo "Simón Rodríguez"</h1>
            <p class="text-lg mb-8 text-blue-100">Fortaleciendo el aprendizaje de 3er Año en Aricagua.</p>
            <div class="flex flex-wrap justify-center gap-4">
                <button onclick="switchTab('canaima')" id="btn-canaima" class="bg-white text-blue-700 px-6 py-2 rounded-full font-bold shadow-lg">Modo Canaima</button>
                <button onclick="switchTab('windows')" id="btn-windows" class="bg-blue-900 text-white px-6 py-2 rounded-full font-bold shadow-lg opacity-80">Modo Windows</button>
            </div>
        </div>
    </header>

    <section class="py-12 max-w-7xl mx-auto px-4">
        <div class="grid md:grid-cols-3 gap-6">
            <div class="bg-white p-6 rounded-xl shadow-sm border border-gray-100 text-center hover:shadow-md transition">
                <i class="fas fa-calculator text-blue-600 text-3xl mb-4"></i>
                <h3 class="font-bold text-lg mb-2">Matemática</h3>
                <p class="text-sm text-gray-500 mb-4">Ecuaciones y funciones paso a paso.</p>
                <a href="#area-estudio" class="inline-block bg-blue-50 text-blue-700 px-4 py-2 rounded-lg font-semibold text-sm">Ver Lecciones ↓</a>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-sm border border-gray-100 text-center hover:shadow-md transition">
                <i class="fas fa-atom text-green-600 text-3xl mb-4"></i>
                <h3 class="font-bold text-lg mb-2">Física</h3>
                <p class="text-sm text-gray-500 mb-4">Movimiento Rectilíneo Uniforme (MRU).</p>
                <a href="#area-estudio" class="inline-block bg-green-50 text-green-700 px-4 py-2 rounded-lg font-semibold text-sm">Explorar Experimentos ↓</a>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-sm border border-gray-100 text-center hover:shadow-md transition">
                <i class="fas fa-vial text-purple-600 text-3xl mb-4"></i>
                <h3 class="font-bold text-lg mb-2">Química</h3>
                <p class="text-sm text-gray-500 mb-4">Tabla periódica y enlaces químicos.</p>
                <a href="#area-estudio" class="inline-block bg-purple-50 text-purple-700 px-4 py-2 rounded-lg font-semibold text-sm">Ver Reacciones ↓</a>
            </div>
        </div>
    </section>

    <main class="max-w-7xl mx-auto px-4 mb-16">
        <div id="content-canaima" class="bg-blue-50 p-6 rounded-2xl border-l-8 border-blue-600 mb-8">
            <h2 class="font-bold text-blue-900 text-xl mb-2"><i class="fab fa-linux mr-2"></i> Guía para Canaima (Software Libre)</h2>
            <p class="text-sm text-blue-700">Utiliza la terminal: <code>sudo apt install gnuplot kalzium geogebra</code></p>
        </div>

        <div id="content-windows" class="hidden bg-sky-50 p-6 rounded-2xl border-l-8 border-sky-600 mb-8">
            <h2 class="font-bold text-sky-900 text-xl mb-2"><i class="fab fa-windows mr-2"></i> Guía para Windows</h2>
            <p class="text-sm text-sky-700">Descarga instaladores oficiales .exe y ejecuta como administrador.</p>
        </div>

        <section id="area-estudio" class="bg-white p-8 rounded-3xl shadow-sm border border-gray-100">
            <h2 class="text-2xl font-bold text-center mb-8">Contenidos Educativos de 3er Año</h2>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="border p-4 rounded-xl">
                    <h4 class="font-bold text-blue-600 border-b pb-2 mb-4">Matemática: Ecuación de 2do Grado</h4>
                    <p class="text-sm bg-gray-50 p-3 rounded font-mono italic text-center">ax² + bx + c = 0</p>
                    <p class="text-xs mt-2 text-gray-500">Ejemplo: Resolver x² - 5x + 6 = 0</p>
                </div>
                <div class="border p-4 rounded-xl">
                    <h4 class="font-bold text-green-600 border-b pb-2 mb-4">Física: Fórmula del MRU</h4>
                    <p class="text-sm bg-gray-50 p-3 rounded font-mono italic text-center">v = d / t</p>
                    <p class="text-xs mt-2 text-gray-500">Velocidad es igual a distancia sobre tiempo.</p>
                </div>
            </div>
        </section>
    </main>

    <section class="max-w-4xl mx-auto px-4 mb-20">
        <div class="bg-slate-800 text-white p-8 rounded-3xl shadow-2xl">
            <h3 class="text-xl font-bold mb-4"><i class="fas fa-check-circle mr-2 text-green-400"></i> Verificador de Enlaces</h3>
            <form id="submissionForm" class="flex flex-col sm:flex-row gap-4 mb-6">
                <input type="text" id="progName" placeholder="Programa" required class="flex-1 p-3 rounded-lg text-slate-900 outline-none">
                <input type="url" id="progLink" placeholder="Link (URL)" required class="flex-1 p-3 rounded-lg text-slate-900 outline-none">
                <button type="submit" class="bg-blue-600 px-6 py-3 rounded-lg font-bold hover:bg-blue-700 transition">Verificar</button>
            </form>
            <div id="resourceContainer" class="space-y-3 max-h-60 overflow-y-auto pr-2">
                </div>
        </div>
    </section>

    <div id="loginModal" class="fixed inset-0 bg-black/80 hidden flex items-center justify-center z-[100] p-4">
        <div class="bg-white rounded-2xl p-8 w-full max-w-sm">
            <h3 class="text-xl font-bold mb-4 text-center">Acceso Investigador</h3>
            <input type="password" id="adminPass" placeholder="Clave Maestra" class="w-full p-4 bg-slate-100 rounded-xl mb-4 border focus:ring-2 focus:ring-blue-500 outline-none">
            <button onclick="login()" class="w-full bg-blue-600 text-white py-3 rounded-xl font-bold mb-2">Entrar</button>
            <button onclick="toggleAdminLogin()" class="w-full text-slate-400 text-sm">Cerrar</button>
        </div>
    </div>

    <footer class="bg-white border-t py-12 text-center">
        <p class="font-bold text-slate-800">Cova W. & Hernández Y.</p>
        <p class="text-slate-500 text-sm">Proyecto de Grado - Técnico Medio en Sistemas</p>
        <p class="text-slate-400 text-[10px] mt-4 uppercase tracking-widest">Aricagua 2026</p>
    </footer>

    <script>
        let resources = [];
        let isAdmin = false;
        const MASTER_PASS = "aricagua2024";

        function switchTab(os) {
            const canaima = document.getElementById('content-canaima');
            const windows = document.getElementById('content-windows');
            const btnC = document.getElementById('btn-canaima');
            const btnW = document.getElementById('btn-windows');

            if(os === 'canaima') {
                canaima.classList.remove('hidden'); windows.classList.add('hidden');
                btnC.classList.add('bg-white', 'text-blue-700'); btnC.classList.remove('bg-blue-900', 'text-white', 'opacity-80');
                btnW.classList.add('bg-blue-900', 'text-white', 'opacity-80'); btnW.classList.remove('bg-white', 'text-blue-700');
            } else {
                windows.classList.remove('hidden'); canaima.classList.add('hidden');
                btnW.classList.add('bg-white', 'text-blue-700'); btnW.classList.remove('bg-blue-900', 'text-white', 'opacity-80');
                btnC.classList.add('bg-blue-900', 'text-white', 'opacity-80'); btnC.classList.remove('bg-white', 'text-blue-700');
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
            renderResources();
            e.target.reset();
        };

        function renderResources() {
            const container = document.getElementById('resourceContainer');
            container.innerHTML = '';
            resources.forEach(res => {
                const div = document.createElement('div');
                div.className = "bg-slate-700 p-4 rounded-xl flex justify-between items-center border border-slate-600";
                div.innerHTML = `
                    <div>
                        <p class="font-bold text-sm text-blue-300">${res.name}</p>
                        <p class="text-[10px] text-slate-400 truncate max-w-[150px]">${res.link}</p>
                    </div>
                    <div class="flex gap-2">
                        <span class="text-[10px] px-2 py-1 rounded bg-slate-800">${res.status}</span>
                        ${isAdmin ? `<button onclick="approve(${res.id})" class="text-green-400 text-xs"><i class="fas fa-check"></i></button>` : ''}
                        ${isAdmin ? `<button onclick="deleteRes(${res.id})" class="text-red-400 text-xs"><i class="fas fa-trash"></i></button>` : ''}
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function toggleAdminLogin() { document.getElementById('loginModal').classList.toggle('hidden'); }

        function login() {
            if(document.getElementById('adminPass').value === MASTER_PASS) {
                isAdmin = true;
                toggleAdminLogin();
                alert("Modo Administrador Activo");
                renderResources();
            } else { alert("Clave Incorrecta"); }
        }

        function approve(id) {
            resources = resources.map(r => r.id === id ? {...r, status: 'Verificado'} : r);
            renderResources();
        }

        function deleteRes(id) {
            resources = resources.filter(r => r.id !== id);
            renderResources();
        }
    </script>
</body>
</html>
