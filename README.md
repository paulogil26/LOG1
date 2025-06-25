        # LOG1
Apresentação Log

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Logística 2025-2030: Cenários Preditivos</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            overflow-x: hidden;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .slide {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            opacity: 0;
            transform: translateY(50px);
            animation: slideIn 1.5s ease-out forwards;
            margin-bottom: 50px;
            padding: 40px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        @keyframes slideIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .slide:nth-child(2) { animation-delay: 0.5s; }
        .slide:nth-child(3) { animation-delay: 1s; }
        .slide:nth-child(4) { animation-delay: 1.5s; }
        .slide:nth-child(5) { animation-delay: 2s; }

        h1 {
            font-size: 3.5rem;
            font-weight: bold;
            text-align: center;
            margin-bottom: 30px;
            background: linear-gradient(45deg, #ff6b6b, #feca57, #48dbfb, #ff9ff3);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientShift 3s ease-in-out infinite;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        h2 {
            font-size: 2.5rem;
            margin-bottom: 25px;
            text-align: center;
            color: #feca57;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: #48dbfb;
            border-left: 4px solid #48dbfb;
            padding-left: 15px;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 30px 0;
            width: 100%;
        }

        .stat-card {
            background: linear-gradient(135deg, rgba(255,255,255,0.2), rgba(255,255,255,0.1));
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255,255,255,0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .stat-card:hover {
            transform: translateY(-10px) scale(1.05);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }

        .stat-number {
            font-size: 3rem;
            font-weight: bold;
            color: #ff6b6b;
            display: block;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .stat-label {
            font-size: 1.2rem;
            color: #ffffff;
            opacity: 0.9;
        }

        .tech-timeline {
            position: relative;
            max-width: 800px;
            margin: 40px auto;
        }

        .timeline-item {
            position: relative;
            padding: 20px 0;
            margin-left: 40px;
            border-left: 3px solid #48dbfb;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -8px;
            top: 25px;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            background: #feca57;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.2); opacity: 0.7; }
        }

        .timeline-content {
            margin-left: 30px;
            padding: 20px;
            background: rgba(255,255,255,0.1);
            border-radius: 10px;
            backdrop-filter: blur(5px);
        }

        .timeline-year {
            font-size: 1.8rem;
            font-weight: bold;
            color: #feca57;
            margin-bottom: 10px;
        }

        .progress-bar {
            width: 100%;
            height: 20px;
            background: rgba(255,255,255,0.2);
            border-radius: 10px;
            overflow: hidden;
            margin: 15px 0;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, #ff6b6b, #feca57);
            border-radius: 10px;
            animation: fillProgress 3s ease-out forwards;
            transform-origin: left;
        }

        @keyframes fillProgress {
            from { transform: scaleX(0); }
            to { transform: scaleX(1); }
        }

        .highlight-box {
            background: linear-gradient(135deg, #ff6b6b, #feca57);
            padding: 25px;
            border-radius: 15px;
            margin: 25px 0;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { box-shadow: 0 10px 30px rgba(0,0,0,0.3); }
            to { box-shadow: 0 15px 40px rgba(255,107,107,0.4); }
        }

        .opportunity-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .opportunity-card {
            background: linear-gradient(135deg, rgba(72,219,251,0.2), rgba(254,202,87,0.2));
            padding: 25px;
            border-radius: 15px;
            border: 1px solid rgba(255,255,255,0.3);
            transition: all 0.3s ease;
        }

        .opportunity-card:hover {
            transform: translateY(-5px);
            background: linear-gradient(135deg, rgba(72,219,251,0.3), rgba(254,202,87,0.3));
        }

        .floating-icons {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .icon {
            position: absolute;
            font-size: 2rem;
            opacity: 0.1;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        .icon:nth-child(1) { top: 10%; left: 10%; animation-delay: 0s; }
        .icon:nth-child(2) { top: 20%; right: 20%; animation-delay: 1s; }
        .icon:nth-child(3) { bottom: 20%; left: 15%; animation-delay: 2s; }
        .icon:nth-child(4) { bottom: 10%; right: 10%; animation-delay: 3s; }

        .cta-button {
            display: inline-block;
            padding: 15px 30px;
            background: linear-gradient(45deg, #ff6b6b, #feca57);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1.2rem;
            margin: 20px 10px;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.4);
        }

        .data-viz {
            width: 100%;
            max-width: 600px;
            height: 300px;
            margin: 30px auto;
            background: rgba(255,255,255,0.1);
            border-radius: 15px;
            padding: 20px;
            backdrop-filter: blur(5px);
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.5rem; }
            h2 { font-size: 2rem; }
            .stats-grid { grid-template-columns: 1fr; }
            .opportunity-grid { grid-template-columns: 1fr; }
            .slide { padding: 20px; }
        }
    </style>
</head>
<body>
    <div class="floating-icons">
        <div class="icon">🚛</div>
        <div class="icon">📦</div>
        <div class="icon">🤖</div>
        <div class="icon">📊</div>
    </div>

    <div class="container">
        <!-- Slide 1: Título Principal -->
        <div class="slide">
            <h1>LOGÍSTICA 2025-2030</h1>
            <h2>Cenários Preditivos do Futuro</h2>
            <div class="highlight-box">
                <p style="font-size: 1.5rem; font-weight: bold;">🚀 Transformação Acelerada em Curso</p>
                <p>Investimentos em tecnologia crescendo <strong>340%</strong> nos últimos 18 meses</p>
            </div>
            <div class="stats-grid">
                <div class="stat-card">
                    <span class="stat-number">200+</span>
                    <span class="stat-label">Empresas Analisadas</span>
                </div>
                <div class="stat-card">
                    <span class="stat-number">73-89%</span>
                    <span class="stat-label">Probabilidade dos Cenários</span>
                </div>
            </div>
        </div>

        <!-- Slide 2: Panorama por Segmento -->
        <div class="slide">
            <h2>🎯 Cenários por Segmento</h2>
            <div class="opportunity-grid">
                <div class="opportunity-card">
                    <h3>E-commerce Logistics</h3>
                    <div class="stat-number" style="font-size: 2rem;">32%</div>
                    <p><strong>Cenário:</strong> Consolidação através de M&A</p>
                    <p>📈 Volume: +24% a.a.</p>
                    <p>📉 Margem: -3,2%</p>
                    <div class="progress-bar">
                        <div class="progress-fill" style="animation-delay: 1s;"></div>
                    </div>
                </div>
                <div class="opportunity-card">
                    <h3>Cargas Refrigeradas</h3>
                    <div class="stat-number" style="font-size: 2rem;">27%</div>
                    <p><strong>Disrupção:</strong> IoT + Blockchain</p>
                    <p>🔥 Redução de perdas: 89%</p>
                    <p>💰 Crescimento: +18% a.a.</p>
                    <div class="progress-bar">
                        <div class="progress-fill" style="animation-delay: 1.5s;"></div>
                    </div>
                </div>
                <div class="opportunity-card">
                    <h3>Cargas Perigosas</h3>
                    <div class="stat-number" style="font-size: 2rem;">18%</div>
                    <p><strong>Regulação:</strong> Certificação digital</p>
                    <p>⚠️ 40% pequenos operadores eliminados</p>
                    <p>📅 Prazo: até 2026</p>
                    <div class="progress-bar">
                        <div class="progress-fill" style="animation-delay: 2s;"></div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Slide 3: Distribuição Tecnológica -->
        <div class="slide">
            <h2>📊 Maturidade Tecnológica Atual</h2>
            <div class="stats-grid">
                <div class="stat-card">
                    <span class="stat-number">46%</span>
                    <span class="stat-label">Pequeno Porte<br>Score: 3,2/10</span>
                    <div style="color: #ff6b6b; margin-top: 10px;">⚠️ Oportunidade Crítica</div>
                </div>
                <div class="stat-card">
                    <span class="stat-number">34%</span>
                    <span class="stat-label">Médio Porte<br>Score: 5,8/10</span>
                    <div style="color: #feca57; margin-top: 10px;">🔄 Transição Acelerada</div>
                </div>
                <div class="stat-card">
                    <span class="stat-number">12%</span>
                    <span class="stat-label">Grande Porte<br>Score: 7,4/10</span>
                    <div style="color: #48dbfb; margin-top: 10px;">👑 Liderança Estabelecida</div>
                </div>
                <div class="stat-card">
                    <span class="stat-number">8%</span>
                    <span class="stat-label">Micro Porte<br>Score: 1,9/10</span>
                    <div style="color: #ff6b6b; margin-top: 10px;">🚨 Risco de Obsolescência</div>
                </div>
            </div>
        </div>

        <!-- Slide 4: Timeline Tecnológica -->
        <div class="slide">
            <h2>🚀 Roadmap Tecnológico</h2>
            <div class="tech-timeline">
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-year">2025</div>
                        <h3>IoT + Automação</h3>
                        <p>💰 Investimento: R$ 4,7 bi (12% da receita)</p>
                        <p>🤖 Hyperautomation Logística</p>
                        <p>📍 23 cidades com entregas autônomas</p>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-year">2027</div>
                        <h3>IA + Blockchain</h3>
                        <p>💰 Investimento: R$ 8,2 bi (18% da receita)</p>
                        <p>🧠 Digital Twin Logístico</p>
                        <p>🔗 Cold chain 100% rastreável</p>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="timeline-year">2030</div>
                        <h3>Quantum Computing</h3>
                        <p>💰 Investimento: R$ 13,1 bi (25% da receita)</p>
                        <p>⚛️ Otimização quântica de rotas</p>
                        <p>♻️ Cadeias 100% circulares</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Slide 5: Transformações Inevitáveis -->
        <div class="slide">
            <h2>⚡ As 5 Transformações Inevitáveis</h2>
            <div class="opportunity-grid">
                <div class="opportunity-card">
                    <h3>1. Hiperotimização</h3>
                    <p>IA redefinirá eficiência operacional</p>
                    <div class="stat-number" style="font-size: 1.5rem;">180% ROI</div>
                </div>
                <div class="opportunity-card">
                    <h3>2. Transparência Total</h3>
                    <p>Blockchain criará confiança absoluta</p>
                    <div class="stat-number" style="font-size: 1.5rem;">94% Precisão</div>
                </div>
                <div class="opportunity-card">
                    <h3>3. Sustentabilidade</h3>  
                    <p>Neutralidade carbono mandatória</p>
                    <div class="stat-number" style="font-size: 1.5rem;">R$ 2,8bi</div>
                </div>
                <div class="opportunity-card">
                    <h3>4. Personalização</h3>
                    <p>Logística adaptada ao cliente individual</p>
                    <div class="stat-number" style="font-size: 1.5rem;">35% LaaS</div>
                </div>
                <div class="opportunity-card">
                    <h3>5. Integração Vertical</h3>
                    <p>Fronteiras entre setores desaparecerão</p>
                    <div class="stat-number" style="font-size: 1.5rem;">40% Automação</div>
                </div>
            </div>
        </div>

        <!-- Slide 6: Concentração de Mercado -->
        <div class="slide">
            <h2>📈 Evolução da Concentração</h2>
            <div class="data-viz">
                <div style="text-align: center; padding: 20px;">
                    <h3 style="margin-bottom: 30px;">Controle de Mercado pelas Top Empresas</h3>
                    <div style="display: flex; justify-content: space-around; align-items: end; height: 200px;">
                        <div style="text-align: center;">
                            <div style="width: 60px; background: linear-gradient(to top, #ff6b6b, #feca57); height: 90px; margin: 0 auto 10px; border-radius: 5px; display: flex; align-items: end; justify-content: center; color: white; font-weight: bold;">45%</div>
                            <div>2025<br>Top 20</div>
                        </div>
                        <div style="text-align: center;">
                            <div style="width: 60px; background: linear-gradient(to top, #ff6b6b, #feca57); height: 120px; margin: 0 auto 10px; border-radius: 5px; display: flex; align-items: end; justify-content: center; color: white; font-weight: bold;">60%</div>
                            <div>2027<br>Top 15</div>
                        </div>
                        <div style="text-align: center;">
                            <div style="width: 60px; background: linear-gradient(to top, #ff6b6b, #feca57); height: 146px; margin: 0 auto 10px; border-radius: 5px; display: flex; align-items: end; justify-content: center; color: white; font-weight: bold;">73%</div>
                            <div>2030<br>Top 10</div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="highlight-box">
                <p style="font-size: 1.3rem;">⏰ <strong>Janela de Oportunidade: 18 meses</strong></p>
                <p>Para modernização antes da obsolescência</p>
            </div>
        </div>

        <!-- Slide 7: Call to Action Final -->
        <div class="slide">
            <h1>🎯 O Futuro é Agora</h1>
            <div class="highlight-box">
                <h3 style="margin-bottom: 20px;">Próximos Catalisadores</h3>
                <p>📅 <strong>6 meses:</strong> Última oportunidade para IoT básico</p>
                <p>⚖️ <strong>18 meses:</strong> Marco regulatório blockchain</p>
                <p>🏆 <strong>36 meses:</strong> Eliminação de 40% dos players</p>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <a href="#" class="cta-button">Acelere sua Transformação</a>
                <a href="#" class="cta-button">Análise Personalizada</a>
            </div>
            <div class="stats-grid" style="margin-top: 40px;">
                <div class="stat-card">
                    <span class="stat-number">73%</span>
                    <span class="stat-label">Mercado controlado por Top 10 em 2030</span>
                </div>
                <div class="stat-card">
                    <span class="stat-number">R$ 890M</span>
                    <span class="stat-label">Investimento anual em requalificação</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Adiciona interatividade básica
        document.addEventListener('DOMContentLoaded', function() {
            // Anima números quando visíveis
            const statNumbers = document.querySelectorAll('.stat-number');
            
            function animateNumbers() {
                statNumbers.forEach(number => {
                    const rect = number.getBoundingClientRect();
                    if (rect.top < window.innerHeight && rect.bottom > 0) {
                        number.style.animation = 'pulse 2s ease-in-out infinite';
                    }
                });
            }

            window.addEventListener('scroll', animateNumbers);
            animateNumbers(); // Chama uma vez no carregamento

            // Adiciona efeito de parallax suave aos ícones flutuantes
            window.addEventListener('scroll', function() {
                const scrollY = window.scrollY;
                const icons = document.querySelectorAll('.icon');
                
                icons.forEach((icon, index) => {
                    const speed = 0.5 + (index * 0.1);
                    icon.style.transform = `translateY(${scrollY * speed}px) rotate(${scrollY * 0.1}deg)`;
                });
            });
        });
    </script>
</body>
</html>
