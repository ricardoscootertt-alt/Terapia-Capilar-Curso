<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Plataforma de Terapia Capilar</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body { background-color: #f8f9fa; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        .hero { background: linear-gradient(135deg, #2c3e50, #00d2ff); color: white; padding: 60px 0; text-align: center; }
        .module-card { border: none; border-radius: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin-bottom: 30px; transition: 0.3s; }
        .module-card:hover { transform: translateY(-5px); }
        .video-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 10px; margin-bottom: 10px; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
        .pdf-section { background-color: #e9ecef; padding: 15px; border-radius: 8px; border-left: 5px solid #00d2ff; }
        .nav-pills .nav-link.active { background-color: #2c3e50; }
        h2 { color: #2c3e50; font-weight: bold; margin-bottom: 25px; border-bottom: 2px solid #00d2ff; display: inline-block; }
    </style>
</head>
<body>

<div class="hero">
    <div class="container">
        <h1>Academia de Terapia Capilar</h1>
        <p class="lead">Formação Profissional Completa</p>
    </div>
</div>

<div class="container mt-5">
    <ul class="nav nav-pills mb-5 justify-content-center" id="pills-tab" role="tablist">
        <li class="nav-item"><button class="nav-link active" data-bs-toggle="pill" data-bs-target="#tricologia">Tricologia Básica</button></li>
        <li class="nav-item"><button class="nav-link" data-bs-toggle="pill" data-bs-target="#eletroterapia">Eletroterapia</button></li>
        <li class="nav-item"><button class="nav-link" data-bs-toggle="pill" data-bs-target="#anamnese">Anamnese</button></li>
        <li class="nav-item"><button class="nav-link" data-bs-toggle="pill" data-bs-target="#argiloterapia">Argiloterapia</button></li>
    </ul>

    <div class="tab-content">
        
        <div class="tab-pane fade show active" id="tricologia">
            <h2>Módulo 1: Tricologia Capilar Básica</h2>
            <div class="row">
                <div class="col-md-6 mb-4">
                    <div class="card module-card p-3">
                        <h5>Abertura e Aula 1</h5>
                        <div class="video-container"><iframe src="https://www.youtube.com/embed/w7YKKS896XM" frameborder="0" allowfullscreen></iframe></div>
                        <div class="video-container"><iframe src="https://www.youtube.com/embed/AsSWz3NfJFE" frameborder="0" allowfullscreen></iframe></div>
                    </div>
                </div>
                <div class="col-md-6 mb-4">
                    <div class="card module-card p-3">
                        <h5>Aulas 2, 3 e 4</h5>
                        <div class="video-container"><iframe src="https://www.youtube.com/embed/3fEafdvQmzo" frameborder="0" allowfullscreen></iframe></div>
                        <div class="video-container"><iframe src="https://www.youtube.com/embed/qYXnvoPCq2Y" frameborder="0" allowfullscreen></iframe></div>
                        <div class="video-container"><iframe src="https://www.youtube.com/embed/r3SRkzYpu90" frameborder="0" allowfullscreen></iframe></div>
                    </div>
                </div>
            </div>
            <div class="pdf-section mb-5">
                <h4>📄 Instruções para PDF (Tricologia)</h4>
                <ul>
                    <li><strong>Conceito:</strong> Estudo da estrutura, funções e patologias do fio e couro cabeludo.</li>
                    <li><strong>Pontos Chave:</strong> Ciclo de crescimento (Anágena, Catágena, Telógena).</li>
                    <li><strong>Dica:</strong> Identifique a haste capilar antes de iniciar qualquer tratamento.</li>
                </ul>
            </div>
        </div>

        <div class="tab-pane fade" id="eletroterapia">
            <h2>Módulo 2: Eletroterapia Capilar</h2>
            <div class="row">
                <div class="col-md-6 mb-4">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/VLR_CrnRicQ" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/EuoQyYa8uEE" frameborder="0" allowfullscreen></iframe></div>
                </div>
                <div class="col-md-6 mb-4">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/SqLtuI0K_98" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/Z6A6pdrLKZY" frameborder="0" allowfullscreen></iframe></div>
                </div>
            </div>
            <div class="pdf-section mb-5">
                <h4>📄 Instruções para PDF (Eletroterapia)</h4>
                <ul>
                    <li><strong>Equipamentos:</strong> Alta Frequência, Laserterapia e LED.</li>
                    <li><strong>Aplicação:</strong> Aumentar a permeabilidade de ativos e bactericida.</li>
                    <li><strong>Segurança:</strong> Contraindicações em gestantes e portadores de marcapasso.</li>
                </ul>
            </div>
        </div>

        <div class="tab-pane fade" id="anamnese">
            <h2>Módulo 3: Anamnese</h2>
            <div class="row">
                <div class="col-md-4 mb-4">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/9HNwZX8p7tM" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/S2hTQx8gFxw" frameborder="0" allowfullscreen></iframe></div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/oCaXLuGRQxc" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/WGCisEZ6etA" frameborder="0" allowfullscreen></iframe></div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/atoET3dyh6Y" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/yRqQ2V2HEW8" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/w_2syoXPglM" frameborder="0" allowfullscreen></iframe></div>
                </div>
            </div>
            <div class="pdf-section mb-5">
                <h4>📄 Instruções para PDF (Anamnese)</h4>
                <ul>
                    <li><strong>Protocolo:</strong> Escuta ativa do paciente e histórico clínico.</li>
                    <li><strong>Exame Visual:</strong> Uso do dermatoscópio para análise do óstio folicular.</li>
                    <li><strong>Checklist:</strong> Hábitos alimentares, estresse e uso de medicamentos.</li>
                </ul>
            </div>
        </div>

        <div class="tab-pane fade" id="argiloterapia">
            <h2>Módulo 4: Argiloterapia</h2>
            <div class="row">
                <div class="col-md-6">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/c3kn6ZVx9Ok" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/GZm804PkavY" frameborder="0" allowfullscreen></iframe></div>
                </div>
                <div class="col-md-6">
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/ZCi6fy-5C2E" frameborder="0" allowfullscreen></iframe></div>
                    <div class="video-container"><iframe src="https://www.youtube.com/embed/cbjwb3ggAa8" frameborder="0" allowfullscreen></iframe></div>
                </div>
            </div>
            <div class="pdf-section mb-5">
                <h4>📄 Instruções para PDF (Argiloterapia)</h4>
                <ul>
                    <li><strong>Tipos:</strong> Argila Verde (oleosidade), Branca (sensibilidade), Preta (desintoxicação).</li>
                    <li><strong>Preparação:</strong> Mistura com hidrolatos ou água mineral (não metal).</li>
                    <li><strong>Aplicação:</strong> Apenas no couro cabeludo, remover antes de secar totalmente.</li>
                </ul>
            </div>
        </div>

    </div>
</div>

<footer class="text-center py-4 mt-5 bg-dark text-white">
    <p>&copy; 2024 Plataforma Terapia Capilar - Todos os direitos reservados.</p>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
