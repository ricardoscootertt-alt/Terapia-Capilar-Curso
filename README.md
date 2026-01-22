# Terapia-Capilar-Curso
Curso para Terapeuta Capilar 
<!DOCTYPE html>
<html lang="pt-pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Terapia Capilar PRO Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .video-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 12px; }
        .tab-content { display: none; }
        .tab-content.active { display: block; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800">

    <!-- Navegação -->
    <nav class="bg-white border-b border-slate-200 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 h-18 flex items-center justify-between py-4">
            <div class="flex items-center gap-2 cursor-pointer" onclick="showTab('home')">
                <i class="fas fa-graduation-cap text-emerald-600 text-2xl"></i>
                <span class="font-bold text-xl tracking-tight text-slate-900">Terapia Capilar <span class="text-emerald-600">PRO</span></span>
            </div>
            <div class="hidden md:flex gap-8 font-semibold text-sm text-slate-600">
                <button onclick="showTab('home')" class="hover:text-emerald-600 transition-colors">Módulos</button>
                <button onclick="showTab('simulator')" class="hover:text-emerald-600 transition-colors">Simulador</button>
                <button onclick="showTab('resources')" class="hover:text-emerald-600 transition-colors">Biblioteca</button>
            </div>
            <button class="bg-emerald-600 text-white px-5 py-2 rounded-full text-sm font-bold hover:bg-emerald-700 transition-all shadow-md">Acesso Aluno</button>
        </div>
    </nav>

    <!-- Header Hero -->
    <header class="bg-white border-b border-slate-200 py-12 mb-8">
        <div class="max-w-7xl mx-auto px-4">
            <h1 class="text-4xl md:text-5xl font-extrabold text-slate-900 mb-4 text-center md:text-left">Curso Completo de Terapia Capilar</h1>
            <p class="text-lg text-slate-600 max-w-3xl text-center md:text-left leading-relaxed">Domine as técnicas de tricologia, patologias do couro cabeludo e eletroterapia com especialistas reais.</p>
        </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 pb-20">

        <!-- ABA: HOME / MÓDULOS -->
        <section id="home" class="tab-content active">
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 mb-12" id="modules-grid">
                <!-- Módulo 1 -->
                <div onclick="openLesson('bio')" class="bg-white p-6 rounded-2xl border border-slate-200 hover:border-emerald-500 hover:shadow-xl transition-all cursor-pointer group">
                    <div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-xl flex items-center justify-center mb-4 group-hover:bg-emerald-600 group-hover:text-white transition-all">
                        <i class="fas fa-dna text-xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Tricologia Básica</h3>
                    <p class="text-sm text-slate-500">Biologia do fio e ciclos de crescimento capilar.</p>
                </div>

                <!-- Módulo 2 -->
                <div onclick="openLesson('micro')" class="bg-white p-6 rounded-2xl border border-slate-200 hover:border-emerald-500 hover:shadow-xl transition-all cursor-pointer group">
                    <div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-xl flex items-center justify-center mb-4 group-hover:bg-emerald-600 group-hover:text-white transition-all">
                        <i class="fas fa-microscope text-xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Tricoscopia</h3>
                    <p class="text-sm text-slate-500">Como realizar exames com micro-câmara e diagnosticar.</p>
                </div>

                <!-- Módulo 3 -->
                <div onclick="openLesson('eletro')" class="bg-white p-6 rounded-2xl border border-slate-200 hover:border-emerald-500 hover:shadow-xl transition-all cursor-pointer group">
                    <div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-xl flex items-center justify-center mb-4 group-hover:bg-emerald-600 group-hover:text-white transition-all">
                        <i class="fas fa-bolt text-xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Eletroterapia</h3>
                    <p class="text-sm text-slate-500">Laser de baixa potência e Alta Frequência na prática.</p>
                </div>

                <!-- Módulo 4 -->
                <div onclick="openLesson('argila')" class="bg-white p-6 rounded-2xl border border-slate-200 hover:border-emerald-500 hover:shadow-xl transition-all cursor-pointer group">
                    <div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-xl flex items-center justify-center mb-4 group-hover:bg-emerald-600 group-hover:text-white transition-all">
                        <i class="fas fa-leaf text-xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Argiloterapia</h3>
                    <p class="text-sm text-slate-500">Detox capilar e óleos essenciais para terapia.</p>
                </div>
            </div>

            <!-- Área de Vídeo Aula (Escondida por padrão) -->
            <div id="lesson-viewer" class="hidden animate-in fade-in duration-500">
                <button onclick="closeLesson()" class="mb-6 text-slate-500 hover:text-emerald-600 font-semibold flex items-center gap-2">
                    <i class="fas fa-arrow-left"></i> Voltar aos Módulos
                </button>
                <div class="grid lg:grid-cols-3 gap-8">
                    <div class="lg:col-span-2 space-y-6">
                        <div class="video-container shadow-2xl bg-black rounded-xl">
                            <iframe id="main-video" src="" frameborder="0" allowfullscreen></iframe>
                        </div>
                        <div class="bg-white p-8 rounded-2xl border border-slate-200">
                            <h2 id="lesson-title" class="text-2xl font-bold mb-4 text-slate-900">Título da Aula</h2>
                            <p class="text-slate-600 leading-relaxed">Nesta aula prática, aprenda os fundamentos e a aplicação técnica para resultados profissionais imediatos.</p>
                        </div>
                    </div>
                    <div class="space-y-6">
                        <div class="bg-emerald-600 text-white p-6 rounded-2xl">
                            <h4 class="font-bold mb-3 flex items-center gap-2"><i class="fas fa-info-circle"></i> Nota da Especialista</h4>
                            <p class="text-sm text-emerald-50/90 leading-relaxed">Lembre-se que a biossegurança é fundamental. Use sempre luvas e esterilize os seus equipamentos após cada atendimento.</p>
                        </div>
                        <div class="bg-white p-6 rounded-2xl border border-slate-200">
                            <h4 class="font-bold mb-4">Material de Apoio</h4>
                            <button class="w-full flex items-center justify-between p-3 bg-slate-50 rounded-lg text-sm hover:bg-slate-100 transition-all mb-2 font-medium">
                                <span><i class="far fa-file-pdf mr-2 text-red-500"></i> Guia de Protocolos</span>
                                <i class="fas fa-download text-slate-400"></i>
                            </button>
                            <button class="w-full flex items-center justify-between p-3 bg-slate-50 rounded-lg text-sm hover:bg-slate-100 transition-all font-medium">
                                <span><i class="far fa-file-pdf mr-2 text-red-500"></i> Dicionário de Ativos</span>
                                <i class="fas fa-download text-slate-400"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- ABA: SIMULADOR -->
        <section id="simulator" class="tab-content max-w-3xl mx-auto">
            <div class="text-center mb-10">
                <h2 class="text-3xl font-bold mb-3">Simulador de Diagnóstico</h2>
                <p class="text-slate-500">Aplique o seu conhecimento clínico para resolver casos reais.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl border border-slate-200 shadow-sm relative overflow-hidden">
                <div class="absolute top-0 left-0 w-2 h-full bg-emerald-500"></div>
                <span class="inline-block bg-slate-100 text-slate-600 text-xs font-bold px-3 py-1 rounded-full mb-4 uppercase tracking-wider">Caso Clínico #01</span>
                <h3 class="text-xl font-bold mb-6 text-slate-900 leading-snug">"Paciente masculino, 35 anos, apresenta rarefação na zona da coroa e entradas frontais. Relata que o pai e o avô têm o mesmo padrão."</h3>
                
                <div class="space-y-4">
                    <button onclick="checkAnswer(true, 'Correto! Trata-se de Alopecia Androgenética (calvície), caracterizada pela miniaturização folicular mediada pela DHT.')" class="w-full text-left p-4 rounded-xl border border-slate-200 hover:border-emerald-500 hover:bg-emerald-50 transition-all font-medium flex justify-between items-center group">
                        <span>A) Alopecia Androgenética</span>
                        <i class="fas fa-chevron-right text-slate-300 group-hover:text-emerald-500"></i>
                    </button>
                    <button onclick="checkAnswer(false, 'Incorreto. A Alopecia Areata costuma apresentar-se em clareiras circulares súbitas.')" class="w-full text-left p-4 rounded-xl border border-slate-200 hover:border-emerald-500 hover:bg-emerald-50 transition-all font-medium flex justify-between items-center group">
                        <span>B) Alopecia Areata</span>
                        <i class="fas fa-chevron-right text-slate-300 group-hover:text-emerald-500"></i>
                    </button>
                    <button onclick="checkAnswer(false, 'Incorreto. O eflúvio telógeno causa uma queda difusa por todo o couro cabeludo, não apenas em zonas específicas.')" class="w-full text-left p-4 rounded-xl border border-slate-200 hover:border-emerald-500 hover:bg-emerald-50 transition-all font-medium flex justify-between items-center group">
                        <span>C) Eflúvio Telógeno</span>
                        <i class="fas fa-chevron-right text-slate-300 group-hover:text-emerald-500"></i>
                    </button>
                </div>
                <div id="feedback" class="mt-8 p-4 rounded-xl hidden"></div>
            </div>
        </section>

        <!-- ABA: BIBLIOTECA -->
        <section id="resources" class="tab-content">
            <h2 class="text-3xl font-bold mb-8">Biblioteca de Referência</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-1 rounded-2xl border border-slate-200 shadow-sm">
                    <img src="https://img.youtube.com/vi/j65R3rYp9oE/maxresdefault.jpg" class="w-full h-48 object-cover rounded-xl" alt="Anatomia">
                    <div class="p-4">
                        <h4 class="font-bold mb-2">Anatomia do Fio</h4>
                        <a href="https://www.youtube.com/watch?v=j65R3rYp9oE" target="_blank" class="text-emerald-600 text-sm font-bold flex items-center gap-1">
                            Ver no YouTube <i class="fas fa-external-link-alt text-xs"></i>
                        </a>
                    </div>
                </div>
                <div class="bg-white p-1 rounded-2xl border border-slate-200 shadow-sm">
                    <img src="https://img.youtube.com/vi/0X7W9G4HqP8/maxresdefault.jpg" class="w-full h-48 object-cover rounded-xl" alt="Tricoscopia">
                    <div class="p-4">
                        <h4 class="font-bold mb-2">Prática de Tricoscopia</h4>
                        <a href="https://www.youtube.com/watch?v=0X7W9G4HqP8" target="_blank" class="text-emerald-600 text-sm font-bold flex items-center gap-1">
                            Ver no YouTube <i class="fas fa-external-link-alt text-xs"></i>
                        </a>
                    </div>
                </div>
                <div class="bg-white p-1 rounded-2xl border border-slate-200 shadow-sm">
                    <img src="https://img.youtube.com/vi/xS8K6P8Kk6Y/maxresdefault.jpg" class="w-full h-48 object-cover rounded-xl" alt="Alta Frequência">
                    <div class="p-4">
                        <h4 class="font-bold mb-2">Uso da Alta Frequência</h4>
                        <a href="https://www.youtube.com/watch?v=xS8K6P8Kk6Y" target="_blank" class="text-emerald-600 text-sm font-bold flex items-center gap-1">
                            Ver no YouTube <i class="fas fa-external-link-alt text-xs"></i>
                        </a>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-white border-t border-slate-200 py-12">
        <div class="max-w-7xl mx-auto px-4 flex flex-col md:flex-row justify-between items-center gap-6">
            <div class="flex items-center gap-2">
                <i class="fas fa-graduation-cap text-emerald-600"></i>
                <span class="font-bold text-slate-900">Terapia Capilar Academy</span>
            </div>
            <p class="text-slate-400 text-sm">© 2024 Formação Profissional em Tricologia. Todos os direitos reservados.</p>
            <div class="flex gap-4 text-slate-400">
                <i class="fab fa-instagram hover:text-emerald-600 cursor-pointer transition-all"></i>
                <i class="fab fa-youtube hover:text-emerald-600 cursor-pointer transition-all"></i>
                <i class="fab fa-linkedin hover:text-emerald-600 cursor-pointer transition-all"></i>
            </div>
        </div>
    </footer>

    <script>
        const lessons = {
            bio: {
                title: "Anatomia e Fisiologia do Fio",
                video: "https://www.youtube.com/embed/j65R3rYp9oE"
            },
            micro: {
                title: "Análise por Tricoscopia Digital",
                video: "https://www.youtube.com/embed/0X7W9G4HqP8"
            },
            eletro: {
                title: "Alta Frequência na Terapia Capilar",
                video: "https://www.youtube.com/embed/xS8K6P8Kk6Y"
            },
            argila: {
                title: "Argiloterapia e Desintoxicação",
                video: "https://www.youtube.com/embed/S2qY4v1X8mQ"
            }
        };

        function showTab(tabId) {
            // Esconder conteúdos das abas
            document.querySelectorAll('.tab-content').forEach(tab => {
                tab.classList.remove('active');
            });
            // Mostrar aba selecionada
            document.getElementById(tabId).classList.add('active');
            
            // Se voltar para home, garantir que os módulos aparecem e o vídeo desaparece
            if(tabId === 'home') {
                closeLesson();
            }
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function openLesson(lessonKey) {
            const lesson = lessons[lessonKey];
            document.getElementById('modules-grid').classList.add('hidden');
            document.getElementById('lesson-viewer').classList.remove('hidden');
            document.getElementById('main-video').src = lesson.video;
            document.getElementById('lesson-title').innerText = lesson.title;
            window.scrollTo({ top: 400, behavior: 'smooth' });
        }

        function closeLesson() {
            document.getElementById('modules-grid').classList.remove('hidden');
            document.getElementById('lesson-viewer').classList.add('hidden');
            document.getElementById('main-video').src = ""; // Parar o vídeo
        }

        function checkAnswer(isCorrect, message) {
            const feedback = document.getElementById('feedback');
            feedback.classList.remove('hidden', 'bg-red-50', 'text-red-700', 'bg-emerald-50', 'text-emerald-700');
            
            if (isCorrect) {
                feedback.classList.add('bg-emerald-50', 'text-emerald-700');
                feedback.innerHTML = `<i class="fas fa-check-circle mr-2"></i> ${message}`;
            } else {
                feedback.classList.add('bg-red-50', 'text-red-700');
                feedback.innerHTML = `<i class="fas fa-times-circle mr-2"></i> ${message}`;
            }
        }
    </script>
</body>
</html>
