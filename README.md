
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visão Geral & Comparativo: Sistemas Tradicionais vs. Sistema EMESP (Rafael Barbosa)</title>
    <style>
        :root {
            --bg-color: #07090f;
            --panel-bg: #0d131f;
            --accent-green: #10b981;
            --accent-amber: #f59e0b;
            --accent-red: #ef4444;
            --accent-blue: #3b82f6;
            --text-main: #f3f4f6;
            --text-muted: #9ca3af;
            --border-color: #1e293b;
        }
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Courier New', Courier, monospace;
        }
        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            padding: 15px;
        }
        header {
            background: var(--panel-bg);
            border: 1px solid var(--border-color);
            padding: 15px 20px;
            margin-bottom: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-radius: 6px;
        }
        header h1 {
            font-size: 1.02rem;
            color: var(--accent-green);
            letter-spacing: 1px;
        }
        .badge {
            background: rgba(16, 185, 129, 0.12);
            color: var(--accent-green);
            border: 1px solid var(--accent-green);
            padding: 6px 12px;
            border-radius: 4px;
            font-size: 0.72rem;
            font-weight: bold;
        }
        .main-container {
            display: grid;
            grid-template-columns: 1.15fr 0.85fr;
            gap: 15px;
            flex: 1;
        }
        @media(max-width: 1150px) {
            .main-container {
                grid-template-columns: 1fr;
            }
        }
        .panel {
            background: var(--panel-bg);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 15px;
            display: flex;
            flex-direction: column;
            gap: 12px;
        }
        .panel-title {
            font-size: 0.83rem;
            color: var(--accent-amber);
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 8px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        .overview-box {
            font-size: 0.75rem;
            line-height: 1.4;
            color: var(--text-muted);
            background: #090d16;
            padding: 10px;
            border-radius: 4px;
            border-left: 3px solid var(--accent-blue);
        }
        /* Tabela Comparativa */
        .comparison-table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.71rem;
            margin-bottom: 5px;
        }
        .comparison-table th, .comparison-table td {
            border: 1px solid var(--border-color);
            padding: 6px;
            text-align: left;
        }
        .comparison-table th {
            background: #111a2c;
            color: var(--text-main);
        }
        .col-traditional {
            color: var(--accent-red);
            background: rgba(239, 68, 68, 0.04);
        }
        .col-emesp {
            color: var(--accent-green);
            background: rgba(16, 185, 129, 0.04);
            font-weight: bold;
        }
        .canvas-wrapper {
            position: relative;
            background: #020408;
            border: 1px solid var(--border-color);
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 4px;
            flex: 1;
            min-height: 280px;
        }
        canvas {
            display: block;
            cursor: crosshair;
        }
        .controls-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 8px;
        }
        button {
            background: #1e293b;
            color: var(--text-main);
            border: 1px solid var(--border-color);
            padding: 9px 12px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 0.76rem;
            transition: all 0.2s;
        }
        button:hover {
            background: #334155;
            border-color: var(--accent-green);
            color: var(--accent-green);
        }
        button.active {
            background: rgba(16, 185, 129, 0.2);
            border-color: var(--accent-green);
            color: var(--accent-green);
        }
        .telemetry-box {
            background: #04060a;
            border: 1px solid var(--border-color);
            padding: 10px;
            border-radius: 4px;
            font-size: 0.76rem;
            display: flex;
            flex-direction: column;
            gap: 5px;
        }
        .telemetry-row {
            display: flex;
            justify-content: space-between;
        }
        .serial-console {
            background: #020305;
            color: var(--accent-green);
            border: 1px solid var(--border-color);
            padding: 8px;
            border-radius: 4px;
            font-size: 0.68rem;
            height: 85px;
            overflow-y: auto;
            white-space: pre-wrap;
        }
    </style>
</head>
<body>

    <header>
        <div>
            <h1>VISÃO GERAL DO APLICATIVO & COMPARAÇÃO TÉCNICA</h1>
            <p style="font-size: 0.69rem; color: var(--text-muted);">Sistemas Tradicionais vs. Sistema EMESP (Rafael Barbosa)</p>
        </div>
        <div class="badge">SISTEMA EMESP: ATIVO</div>
    </header>

    <div class="main-container">
        <!-- Coluna Esquerda: Visão Geral e Tabela Comparativa -->
        <div class="panel">
            <div class="panel-title">Visão Geral do Aplicativo & Memorial Descritivo</div>
            <div class="overview-box">
                <strong>Visão Geral:</strong> O aplicativo gerencia e demonstra o <strong>Sistema EMESP (desenvolvido por Rafael Barbosa)</strong>, que revoluciona o monitoramento convertendo câmeras legadas em sensores inteligentes autônomos. Utiliza IA de borda com servomecanismos em malha fechada, eliminando a sobrecarga cognitiva humana, reduzindo o tempo de resposta para menos de 15 milissegundos e protegendo os dados com criptografia pós-quântica (PQC Kyber-1024 e Dilithium-5).
            </div>

            <div class="panel-title" style="margin-top: 4px;">Comparação com Sistemas Atuais</div>
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Característica / Parâmetro</th>
                        <th>Sistemas de Monitoramento Tradicionais</th>
                        <th>Sistema EMESP (Rafael Barbosa)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Operação de Câmeras Legadas</strong></td>
                        <td class="col-traditional">Estática e isolada (requer substituição por câmeras PTZ caras)</td>
                        <td class="col-emesp">Dinâmica e integrada (transforma câmeras antigas em sensores inteligentes)</td>
                    </tr>
                    <tr>
                        <td><strong>Intervenção Humana</strong></td>
                        <td class="col-traditional">100% manual (operador precisa alternar feeds de vídeo no monitor)</td>
                        <td class="col-emesp">100% automatizada por IA e servomecanismos em malha fechada</td>
                    </tr>
                    <tr>
                        <td><strong>Tempo Médio de Resposta</strong></td>
                        <td class="col-traditional">3.5 a 7.0 segundos (tempo de reação e acionamento no rádio)</td>
                        <td class="col-emesp">Menos de 15 milissegundos (sincronização mecânica instantânea)</td>
                    </tr>
                    <tr>
                        <td><strong>Sobrecarga Cognitiva</strong></td>
                        <td class="col-traditional">Altíssima (exige atenção simultânea em múltiplos mosaicos de tela)</td>
                        <td class="col-emesp">Nula (a armação física ou o drone atuam como um ponteiro visual direto)</td>
                    </tr>
                    <tr>
                        <td><strong>Segurança de Comunicação</strong></td>
                        <td class="col-traditional">Criptografia padrão AES (vulnerável a futuros computadores quânticos)</td>
                        <td class="col-emesp">Criptografia PQC (Pós-Quântica) com algoritmos Kyber-1024 e Dilithium-5</td>
                    </tr>
                </tbody>
            </table>

            <div class="controls-grid" style="margin-top: 4px;">
                <button id="btnToggleSim" class="active">Modo Comparativo: Lado a Lado</button>
                <button id="btnTriggerAlert">Disparar Evento de Intrusão</button>
            </div>
        </div>

        <!-- Coluna Direita: Simulador Gráfico Canvas & Telemetria -->
        <div class="panel">
            <div class="panel-title">Simulação Visual: Tradicional vs. EMESP</div>
            <div class="canvas-wrapper">
                <canvas id="simCanvas" width="500" height="260"></canvas>
            </div>

            <div class="panel-title">Telemetria de Desempenho & Criptografia PQC</div>
            <div class="telemetry-box">
                <div class="telemetry-row"><span>Latência Média de Resposta:</span> <span id="valLatency" style="color:var(--accent-green)">12.4 ms (&lt; 15ms)</span></div>
                <div class="telemetry-row"><span>Sobrecarga Cognitiva Humana:</span> <span style="color:var(--accent-green)">Nula [Automação em Malha Fechada]</span></div>
                <div class="telemetry-row"><span>Protocolo de Segurança:</span> <span style="color:var(--accent-blue)">PQC (Kyber-1024 + Dilithium-5)</span></div>
                <div class="telemetry-row"><span>Status de Câmeras Legadas:</span> <span style="color:var(--accent-green)">Integradas como Sensores Inteligentes</span></div>
            </div>

            <div class="panel-title">Log do Sistema EMESP</div>
            <div class="serial-console" id="serialConsole">[INIT] Sistema EMESP (Rafael Barbosa) carregado.
[PQC] Chaves Kyber-1024 e Dilithium-5 ativas.
[AI] Câmeras legadas convertidas em nós inteligentes. Malha fechada operacional.</div>
        </div>
    </div>

    <script>
        const canvas = document.getElementById('simCanvas');
        const ctx = canvas.getContext('2d');

        let alertActive = false;
        let intrusionPos = { x: 380, y: 130 };

        // Elementos da UI
        const btnToggleSim = document.getElementById('btnToggleSim');
        const btnTriggerAlert = document.getElementById('btnTriggerAlert');
        const valLatency = document.getElementById('valLatency');
        const serialConsole = document.getElementById('serialConsole');

        function logMsg(msg) {
            serialConsole.textContent += "\n" + msg;
            serialConsole.scrollTop = serialConsole.scrollHeight;
        }

        btnTriggerAlert.addEventListener('click', () => {
            alertActive = true;
            intrusionPos.x = 100 + Math.random() * 300;
            intrusionPos.y = 50 + Math.random() * 160;
            logMsg("[ALERTA] Intrusão detectada no setor. EMESP responde em < 15ms. Tradicional requer 5.2s.");
            setTimeout(() => { alertActive = false; }, 3500);
        });

        function update() {
            // Atualização contínua da simulação
        }

        function draw() {
            ctx.fillStyle = '#020408';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            // Dividir canvas em duas seções verticais para comparar
            const midX = canvas.width / 2;

            // Linha divisória
            ctx.strokeStyle = '#1e293b';
            ctx.lineWidth = 2;
            ctx.beginPath();
            ctx.moveTo(midX, 0); ctx.lineTo(midX, canvas.height);
            ctx.stroke();

            // Títulos das seções no Canvas
            ctx.fillStyle = '#ef4444';
            ctx.font = '9px Courier New';
            ctx.fillText("SISTEMA TRADICIONAL (Atraso 3.5-7s)", 15, 20);

            ctx.fillStyle = '#10b981';
            ctx.fillText("SISTEMA EMESP (Rafael Barbosa <15ms)", midX + 15, 20);

            // Simulação Esquerda (Tradicional: telas estáticas lentas)
            ctx.strokeStyle = 'rgba(239, 68, 68, 0.4)';
            ctx.strokeRect(20, 35, midX - 35, 200);
            ctx.fillStyle = '#9ca3af';
            ctx.font = '8px Courier New';
            ctx.fillText("Mosaico 1: Operador buscando feed...", 30, 60);
            ctx.fillText("Mosaico 2: Alerta manual pendente...", 30, 80);
            ctx.fillText("Status: Atraso de rádio / 5.2s lag", 30, 110);

            if (alertActive) {
                ctx.fillStyle = 'rgba(239, 68, 68, 0.2)';
                ctx.fillRect(20, 35, midX - 35, 200);
                ctx.fillStyle = '#ef4444';
                ctx.fillText(">>> OPERADOR CONFUSO EM MOSAICOS <<<", 28, 145);
            }

            // Simulação Direita (EMESP: IA e Servomecanismo em malha fechada)
            ctx.strokeStyle = 'rgba(16, 185, 129, 0.5)';
            ctx.strokeRect(midX + 15, 35, midX - 30, 200);
            ctx.fillStyle = '#10b981';
            ctx.fillText("Câmera Legada convertida em Sensor", midX + 25, 60);
            ctx.fillText("Malha Fechada: IA & Servos Ativos", midX + 25, 80);
            ctx.fillText("Criptografia PQC: Kyber-1024 / Dilithium", midX + 25, 100);

            // Alvo / Intruso
            ctx.fillStyle = '#f59e0b';
            ctx.beginPath();
            ctx.arc(midX + 100, 140, 7, 0, Math.PI * 2);
            ctx.fill();
            ctx.fillStyle = '#ffffff';
            ctx.fillText("INTRUSO", midX + 75, 125);

            // Ponteiro visual direto EMESP instantâneo
            ctx.strokeStyle = '#10b981';
            ctx.lineWidth = 1.5;
            ctx.setLineDash([2, 2]);
            ctx.beginPath();
            ctx.moveTo(midX + 40, 180);
            ctx.lineTo(midX + 100, 140);
            ctx.stroke();
            ctx.setLineDash([]);

            ctx.fillStyle = '#10b981';
            ctx.fillText("Tempo de Resposta: 12.4ms [OK]", midX + 25, 215);
        }

        function loop() {
            update();
            draw();
            requestAnimationFrame(loop);
        }

        requestAnimationFrame(loop);
    </script>
</body>
</html>
