<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FemFit - Empoderamiento a través del Fitness</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&display=swap');
        
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            scroll-behavior: smooth;
        }

        .glass-nav {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }

        .hero-gradient {
            background: radial-gradient(circle at top right, #fff1f2, #ffffff);
        }

        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(219, 39, 119, 0.1);
        }
    </style>
</head>
<body class="bg-white text-slate-900">

    <!-- Navegación -->
    <nav class="fixed w-full z-50 glass-nav border-b border-pink-50">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <div class="flex items-center gap-2">
                <div class="w-10 h-10 bg-pink-600 rounded-xl flex items-center justify-center text-white">
                    <i class="fas fa-dumbbell"></i>
                </div>
                <span class="text-2xl font-extrabold tracking-tight text-pink-600">FemFit</span>
            </div>
            
            <div class="hidden md:flex items-center gap-8 font-semibold text-slate-600">
                <a href="#metodo" class="hover:text-pink-600 transition-colors">Método</a>
                <a href="#entrenamientos" class="hover:text-pink-600 transition-colors">Programas</a>
                <a href="#precios" class="hover:text-pink-600 transition-colors">Precios</a>
            </div>

            <div class="flex items-center gap-4">
                <button class="hidden sm:block font-bold text-pink-600 px-4">Iniciar Sesión</button>
                <button class="bg-pink-600 text-white px-6 py-2.5 rounded-full font-bold shadow-lg shadow-pink-200 hover:bg-pink-700 transition-all">
                    Empezar Gratis
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="pt-32 pb-20 px-6 hero-gradient overflow-hidden">
        <div class="max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center">
            <div class="animate-in slide-in-from-left duration-700">
                <span class="bg-pink-100 text-pink-600 px-4 py-1.5 rounded-full text-sm font-bold uppercase tracking-wider">
                    Comunidad Fitness #1 para Mujeres
                </span>
                <h1 class="text-5xl md:text-7xl font-extrabold leading-tight mt-6 mb-8 text-slate-900">
                    Entrena al ritmo de <span class="text-pink-600">tu ciclo</span>
                </h1>
                <p class="text-lg text-slate-600 mb-10 leading-relaxed max-w-lg">
                    FemFit es la primera plataforma que sincroniza tus rutinas de ejercicio con tus fases hormonales para maximizar resultados y cuidar tu salud.
                </p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <button class="bg-slate-900 text-white px-8 py-4 rounded-2xl font-bold flex items-center justify-center gap-2 hover:bg-slate-800 transition-all">
                        <i class="fab fa-apple text-xl"></i> App Store
                    </button>
                    <button class="bg-slate-900 text-white px-8 py-4 rounded-2xl font-bold flex items-center justify-center gap-2 hover:bg-slate-800 transition-all">
                        <i class="fab fa-google-play text-xl"></i> Play Store
                    </button>
                </div>
                <div class="mt-8 flex items-center gap-4">
                    <div class="flex -space-x-3">
                        <img src="https://i.pravatar.cc/100?u=1" class="w-10 h-10 rounded-full border-2 border-white" alt="Usuario">
                        <img src="https://i.pravatar.cc/100?u=2" class="w-10 h-10 rounded-full border-2 border-white" alt="Usuario">
                        <img src="https://i.pravatar.cc/100?u=3" class="w-10 h-10 rounded-full border-2 border-white" alt="Usuario">
                    </div>
                    <p class="text-sm text-slate-500 font-medium">Más de <span class="text-pink-600 font-bold">50,000</span> mujeres ya están entrenando</p>
                </div>
            </div>
            <div class="relative animate-in zoom-in duration-700">
                <div class="absolute -top-10 -left-10 w-40 h-40 bg-pink-200 rounded-full blur-3xl opacity-50"></div>
                <div class="absolute -bottom-10 -right-10 w-60 h-60 bg-rose-200 rounded-full blur-3xl opacity-50"></div>
                <img src="https://images.unsplash.com/photo-1518310383802-640c2de311b2?w=800&auto=format&fit=crop" 
                     class="rounded-[40px] shadow-2xl relative z-10 w-full object-cover aspect-[4/5]" 
                     alt="Entrenamiento FemFit">
                
                <!-- Floating Card -->
                <div class="absolute bottom-10 left-[-20px] bg-white p-4 rounded-2xl shadow-xl z-20 flex items-center gap-4 animate-bounce">
                    <div class="w-12 h-12 bg-green-100 text-green-600 rounded-full flex items-center justify-center">
                        <i class="fas fa-heartbeat"></i>
                    </div>
                    <div>
                        <p class="text-xs text-slate-500 font-bold uppercase tracking-tighter">Energía Hoy</p>
                        <p class="text-lg font-black">Máxima (Día 14)</p>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Metodología -->
    <section id="metodo" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-4xl font-extrabold mb-6">¿Por qué elegir FemFit?</h2>
                <p class="text-slate-600 text-lg">Entendemos que el cuerpo femenino cambia cada semana. Adaptamos la intensidad para que nunca te sientas agotada innecesariamente.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <div class="p-8 bg-slate-50 rounded-[32px] card-hover">
                    <div class="w-14 h-14 bg-pink-100 text-pink-600 rounded-2xl flex items-center justify-center text-2xl mb-6">
                        <i class="fas fa-sync-alt"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Sincronización de Ciclo</h3>
                    <p class="text-slate-600">Algoritmos que ajustan tu plan según tus niveles de estrógeno y progesterona.</p>
                </div>
                <div class="p-8 bg-slate-50 rounded-[32px] card-hover border-2 border-pink-100">
                    <div class="w-14 h-14 bg-pink-600 text-white rounded-2xl flex items-center justify-center text-2xl mb-6">
                        <i class="fas fa-utensils"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Nutrición Hormonal</h3>
                    <p class="text-slate-600">Recetas específicas para combatir antojos y mejorar la digestión en cada fase.</p>
                </div>
                <div class="p-8 bg-slate-50 rounded-[32px] card-hover">
                    <div class="w-14 h-14 bg-pink-100 text-pink-600 rounded-2xl flex items-center justify-center text-2xl mb-6">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Comunidad Exclusiva</h3>
                    <p class="text-slate-600">Comparte logros y dudas en un espacio seguro con miles de mujeres.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Programas Destacados -->
    <section id="entrenamientos" class="py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex justify-between items-end mb-12">
                <div>
                    <h2 class="text-4xl font-extrabold mb-4">Programas Populares</h2>
                    <p class="text-slate-600">Diseñados por expertas en fisiología femenina.</p>
                </div>
                <button class="text-pink-600 font-bold flex items-center gap-2">Ver todos <i class="fas fa-arrow-right"></i></button>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="bg-white rounded-[32px] overflow-hidden shadow-sm group">
                    <div class="h-64 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1544367567-0f2fcb009e0b?w=800&auto=format&fit=crop" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" alt="Yoga">
                    </div>
                    <div class="p-8">
                        <div class="flex justify-between items-center mb-4">
                            <span class="bg-blue-50 text-blue-600 px-3 py-1 rounded-full text-xs font-bold uppercase">Zen</span>
                            <span class="text-slate-400 text-sm"><i class="far fa-clock mr-1"></i> 30 min</span>
                        </div>
                        <h4 class="text-xl font-bold mb-2">Yoga Post-Periodo</h4>
                        <p class="text-slate-500 text-sm mb-6">Ideal para recuperar movilidad y energía suavemente.</p>
                        <button class="w-full py-3 bg-pink-50 text-pink-600 font-bold rounded-xl hover:bg-pink-600 hover:text-white transition-colors">
                            Detalles del programa
                        </button>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="bg-white rounded-[32px] overflow-hidden shadow-sm group border-2 border-pink-50">
                    <div class="h-64 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1517836357463-d25dfeac3438?w=800&auto=format&fit=crop" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" alt="HIIT">
                    </div>
                    <div class="p-8">
                        <div class="flex justify-between items-center mb-4">
                            <span class="bg-orange-50 text-orange-600 px-3 py-1 rounded-full text-xs font-bold uppercase">Alta Intensidad</span>
                            <span class="text-slate-400 text-sm"><i class="far fa-clock mr-1"></i> 20 min</span>
                        </div>
                        <h4 class="text-xl font-bold mb-2">Power Burn HIIT</h4>
                        <p class="text-slate-500 text-sm mb-6">Aprovecha el pico de estrógeno para quemar grasa.</p>
                        <button class="w-full py-3 bg-pink-600 text-white font-bold rounded-xl shadow-lg shadow-pink-100">
                            Empezar ahora
                        </button>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="bg-white rounded-[32px] overflow-hidden shadow-sm group">
                    <div class="h-64 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1574680077505-ef74a4ef527c?w=800&auto=format&fit=crop" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" alt="Fuerza">
                    </div>
                    <div class="p-8">
                        <div class="flex justify-between items-center mb-4">
                            <span class="bg-purple-50 text-purple-600 px-3 py-1 rounded-full text-xs font-bold uppercase">Fuerza</span>
                            <span class="text-slate-400 text-sm"><i class="far fa-clock mr-1"></i> 45 min</span>
                        </div>
                        <h4 class="text-xl font-bold mb-2">Tonificación Glúteos</h4>
                        <p class="text-slate-500 text-sm mb-6">Rutina intensa de pesas para tren inferior.</p>
                        <button class="w-full py-3 bg-pink-50 text-pink-600 font-bold rounded-xl hover:bg-pink-600 hover:text-white transition-colors">
                            Detalles del programa
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-900 text-white py-20">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-4 gap-12">
            <div class="col-span-2">
                <div class="flex items-center gap-2 mb-6">
                    <div class="w-10 h-10 bg-pink-600 rounded-xl flex items-center justify-center">
                        <i class="fas fa-dumbbell"></i>
                    </div>
                    <span class="text-2xl font-extrabold">FemFit</span>
                </div>
                <p class="text-slate-400 max-w-sm mb-8">Empoderando a las mujeres para que tomen control de su salud a través del conocimiento de su propio cuerpo.</p>
                <div class="flex gap-4">
                    <a href="#" class="w-10 h-10 bg-slate-800 rounded-full flex items-center justify-center hover:bg-pink-600 transition-colors"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="w-10 h-10 bg-slate-800 rounded-full flex items-center justify-center hover:bg-pink-600 transition-colors"><i class="fab fa-tiktok"></i></a>
                    <a href="#" class="w-10 h-10 bg-slate-800 rounded-full flex items-center justify-center hover:bg-pink-600 transition-colors"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
            <div>
                <h5 class="font-bold mb-6 text-lg">Compañía</h5>
                <ul class="space-y-4 text-slate-400">
                    <li><a href="#" class="hover:text-white transition-colors">Sobre Nosotras</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Entrenadoras</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Carreras</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Blog</a></li>
                </ul>
            </div>
            <div>
                <h5 class="font-bold mb-6 text-lg">Soporte</h5>
                <ul class="space-y-4 text-slate-400">
                    <li><a href="#" class="hover:text-white transition-colors">Centro de Ayuda</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Contacto</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Privacidad</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Términos</a></li>
                </ul>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-6 mt-20 pt-8 border-t border-slate-800 text-center text-slate-500 text-sm">
            © 2024 FemFit Inc. Todos los derechos reservados. Hecho con ❤️ para ti.
        </div>
    </footer>

</body>
</html>
