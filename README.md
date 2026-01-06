<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Currículo - Ronan Gabriel</title>
    <link rel="icon" href="/favicon.ico" type="image/x-icon">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">

    <!-- Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-ZF9E2WKWQW"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-ZF9E2WKWQW');
    </script>  
    <style>
        :root {
            /* Paleta de Cores Modernizada */
            --primary-text: #1a2a3a; /* Slate Blue profundo para texto */
            --secondary-text: #546e7a; /* Cinza azulado para detalhes */
            --accent-color: #007bff; /* Azul vibrante tech para destaques */
            --bg-body: #f4f7f6;
            --bg-container: #ffffff;
            --bg-skills: #f8f9fa; /* Fundo sutil para skills */
            --section-spacing: 1.8rem;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--primary-text);
            background: var(--bg-body);
            padding: 2rem 1rem;
            font-size: 10pt; /* Tamanho base otimizado para A4 */
        }

        .cv-container {
            max-width: 21cm;
            margin: 0 auto;
            background: var(--bg-container);
            padding: 3rem;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            border-radius: 8px;
        }

        /* Links */
        a {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.2s ease;
        }
        a:hover {
            text-decoration: underline;
            color: #0056b3;
        }

        /* Header */
        header {
            margin-bottom: 2.5rem;
            border-bottom: 1px solid #eee;
            padding-bottom: 2rem;
        }

        h1 {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--primary-text);
            letter-spacing: -0.5px;
            line-height: 1.2;
            margin-bottom: 0.5rem;
        }

        .subtitle {
            font-size: 1.2rem;
            color: var(--accent-color);
            font-weight: 600;
            margin-bottom: 1.2rem;
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem 1.5rem;
            font-size: 0.95rem;
            color: var(--secondary-text);
        }

        .contact-info span {
            display: flex;
            align-items: center;
            gap: 0.3rem;
        }

        /* Sections */
        section {
            margin-bottom: var(--section-spacing);
        }

        h2 {
            font-size: 1.1rem;
            color: var(--accent-color);
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
            margin-bottom: 1.2rem;
            display: flex;
            align-items: center;
        }
        
        /* Opcional: pequena linha ao lado do H2 */
        h2::after {
            content: "";
            flex: 1;
            margin-left: 1rem;
            height: 1px;
            background: #eee;
        }

        /* Professional Summary */
        .summary-text {
            text-align: left;
            color: var(--primary-text);
        }

        /* Skills */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 1rem;
        }

        .skill-category {
            background: var(--bg-skills);
            padding: 1rem;
            border-radius: 6px;
            border-left: 3px solid var(--accent-color);
        }

        .skill-category strong {
            color: var(--primary-text);
            display: block;
            margin-bottom: 0.4rem;
            font-weight: 700;
        }

        /* Experience & Projects */
        .entry {
            margin-bottom: 1.5rem;
        }

        .entry-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-bottom: 0.5rem;
            flex-wrap: wrap;
        }

        .entry-title-group {
            flex: 1;
            min-width: 60%;
        }

        .entry-title {
            font-weight: 700;
            font-size: 1.05rem;
            color: var(--primary-text);
        }

        .sep {
            margin: 0 0.3rem;
            color: var(--accent-color);
        }

        .entry-company {
            font-weight: 600;
            color: var(--accent-color);
        }

        .entry-date {
            font-size: 0.9rem;
            color: var(--secondary-text);
            font-weight: 500;
            white-space: nowrap;
        }

        /* List Items */
        ul {
            list-style-type: none;
            padding-left: 0;
        }

        li {
            position: relative;
            padding-left: 1.5rem;
            margin-bottom: 0.4rem;
            text-align: left; /* Alinhamento à esquerda para melhor leitura */
            color: var(--primary-text);
        }

        li::before {
            content: "•";
            position: absolute;
            left: 0.2rem;
            top: -0.1rem; /* Ajuste fino da posição do bullet */
            color: var(--accent-color);
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* Print Optimization */
        @media print {
            body {
                background: none;
                padding: 0;
                font-size: 9.5pt; /* Ligeira redução para impressão */
            }
            .cv-container {
                box-shadow: none;
                padding: 2.5rem;
                margin: 0;
                width: 100%;
                max-width: none;
                border-radius: 0;
            }
            a {
                text-decoration: none;
                color: var(--primary-text);
            }
            /* Evita que links mostrem a URL na impressão */
            a[href^="http"]:after {
                content: ""; 
            }
            .skill-category {
                border: 1px solid #eee; /* Borda sutil para impressão em P&B */
                background: none !important;
                -webkit-print-color-adjust: exact; 
            }
        }
    </style>
</head>
<body>
    <div class="cv-container">
        <header>
            <h1>Ronan Gabriel </h1>
            <div class="subtitle">Cientista de Dados | Python, SQL & Power BI | Background em IA e ML, BI e Analytics</div>
            <div class="contact-info">
                <span>📍 Brasília, DF (Disponível para Outras Regiões)</span>
                <span>📱 (61) 99363-9187</span>
                <span>📧 <a href="mailto:ronangabriel1@gmail.com">ronangabriel1@gmail.com</a></span>
                <span>🔗 <a href="https://linkedin.com/in/ronangabriel1" target="_blank">linkedin.com/in/ronangabriel1</a></span>
                <span>💻 <a href="https://github.com/ronang4briel" target="_blank">github.com/ronang4briel</a></span>
            </div>
        </header>

        <section>
            <h2>Resumo Profissional</h2>
            <p class="summary-text">
                Meu trabalho consiste em fortalecer as capacidades analíticas da instituição para gerar informações que sirvam de evidências para a tomada de decisões estratégicas. Possuo background e ampla experiência nos seguimentos governamentais da área da saúde e corporativos.
                Atualmente, trabalho desenvolvendo suporte gerencial e analítico para atividades relacionadas à Governança, Inteligência e Ciência de Dados também a implementação de Inteligência Artificial nos proecssos de trabalho das áreas finalísticas utilizando <strong>Python (Pandas, Scikit-learn), SQL e Power BI</strong>.
            </p>
        </section>

        <section>
            <h2>Competências Técnicas</h2>
            <div class="skills-grid">
            <div class="skill-category">
            <strong>Ciência de Dados</strong>
                   Aprendizado de máquina, Deep Learning, IA, Estatistica Preditiva.
                   </div>
                   <div class="skill-category">
                    <strong>Análise de Dados & BI</strong>
                    Python, SQL, Power BI (DAX), Excel Avançado, Estatística Descritiva, ETL/ELT, Web Scraping, Git/GitHub.
                    </div>
                    <div class="skill-category">
                    <strong>Banco de Dados & Cloud</strong>
                    Postgre, SQLserver, Azurefactoring.
                </div>
            </div>
        </section>

        <section>
            <h2>Experiência Profissional</h2>

            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Governança, Ciência e Inteligência de Dados </span> <span class="sep">|</span> <span class="entry-company">CGINT - Anvisa</span>
                    </div>
                    <span class="entry-date">Dez 2022 – Presente</span>
                </div>
                <ul>
                    <li>Apoio gerencial e técnico em atividades de <strong> Ciência, Governmança e Inteligência de dados</strong> realizando levantamento de requisitos, gestão de projetos, escolhas de ferramentas, .</li>
                    <li>Administração e monitoramento de licenciamento de ferramentas de BI e de Processamento em núvem de preojetos de dados.</li>
                    <li>Desenvolvimento de indicadores de desempenho e monitoramento de contratos de BI & Analytics e Azure.</li>
                </ul>
            </div>

            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Analista de Dados</span> <span class="sep">|</span> <span class="entry-company">GECOR - Anvisa</span>
                    </div>
                    <span class="entry-date">Jan 2021– Jul 2022</span>
                </div>
                <ul>
                    <li>Modelagem e processamento de alguns dados monitorados pela Anvisa com otimização na disponibilização ddos abertos em <strong>30%</strong>.</li>
                    <li>Realização de análise exploratória de dados (EDA) de performance de colaboradores identificando gargalos de em projetos e sugerindo intervenções estratégicas de performance baseadas em dados.</li>
                    <li>Desenvolvimento de dashboards publicados no
                    <span> <a href="https://www.gov.br/anvisa/pt-br/assuntos/regulamentacao/observatorio#:~:text=O%20Observat%C3%B3rio%20de%20Regula%C3%A7%C3%A3o%20Sanit%C3%A1ria,de%20forma%20inteligente%20e%20din%C3%A2mica)" target="_blank">Observatório de Regulação da Anvisa</a></span>.</li>
                </ul>
            </div>

            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Analista de Dados</span> <span class="sep">|</span> <span class="entry-company">GELOG - Anvisa</span>
                    </div>
                    <span class="entry-date">Jan 2019 – Jun 2020</span>
                </div>
                <ul>
                    <li>Monitoramento de contratos de logisticas e de outros seguimentos obtendo <strong>redução considerável</strong> em dotações orçamentarias.</li>
                    <li>Desenvolvimento de painéis estratégicos para tomada de decisão estratégicas em contratações da casa.</li>
                </ul>
            </div>

            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Consultor Analista de Dados</span> <span class="sep">|</span> <span class="entry-company">Rede HADC (franquias de fast food)</span>
                    </div>
                    <span class="entry-date">jan 2018 – Dez 2018</span>
                </div>
                <ul>
                    <li>Automação de coleta de dados diários de faturamento, API com paginação.</li>
                    <li>Desenvolvimento de indicadores e regras de negócio em DAX/Power BI aumentando faturamento mensal de <strong> 3% a 5%</strong>.</li>
                    <li>Atuou na modelagem de dados garantindo atualização diária de indicadores de desempenho.</li>
                </ul>
            </div>
        </section>

        <section>
            <h2>Projetos em Destaque</h2>
            <div class="entry">
                <div class="entry-header">
                    <span class="entry-title">IA Aplicada a Análise de compras Públicas </span>
                    <span class="entry-date" style="color: var(--accent-color)">Python, Power BI, SQLserver</span>
                </div>
                <ul>
                    <li><strong>Problema de Negócio:</strong> Identificar discrepância regional e anual em compras públicas e privadas de stents farmacológicos.</li>
                    <li><strong>Solução:</strong>Automação no processamento e ETL de dados do OpenDataSUS utilizando SQL, Python e Power BI.</li>
                    <li><strong>Resultado:</strong> As variáveis análisadas foram capazes de prever aproximadamente 38% do preço das compras, apontando para criticidade regional e logística como resultado.</li>
                </ul>
            </div>
            <div class="entry">
                <div class="entry-header">
                    <span class="entry-title">Ciência de Dados - Predição de Casos Graves (Dengue)</span>
                    <span class="entry-date" style="color: var(--accent-color)">Python, SQL, Power BI</span>
                </div>
                <ul>
                    <li><strong>Problema de Negócio:</strong> Transformar dados brutos governamentais em inteligência preditiva de casos de dengue que poderiam evoluir para casos graves e possivelmente óbitos.</li>
                    <li><strong>Solução:</strong> Criação de pipeline de dadis com ETL automatizado com Python (Pandas), modelagem e dashboard estratégico.</li>
                    <li><strong>Resultado:</strong> Mapeamento da região sudeste segundo dados do SINAN online, otimização e validação do modelo preditivo. (Técnicas de validação como accuracy, recall, precision e cross validation).</li>
                </ul>
            </div>
            <div class="entry">
                <div class="entry-header">
                    <span class="entry-title">Análise de Dados</span>
                    <span class="entry-date" style="color: var(--accent-color)">Python, Excel, PowerBI</span>
                    </div>
                <ul>                
                    <li>Automatização de pipelines de dados <strong>(ETL com python e Power BI)</strong> viabilizando o desenvolvimento de painéis analíticos para acompanhamento de resultado e suporte à tomada de decisão de franquiados de rede de fastfood.</li>
                    <li>Monitoramento contínuo de KPIs de desempenho <strong>(Ticket Médio, Cross Sell por meio de Business Intelligence)</strong> apoiando decisões estratégicas e melhoria de resultados.</li>
                    <li>Análise Estatistica e probabilistica de dados de demissões punitivas do Governo Federal para criação de politicas públicas direcionadas com foco na identificação de <strong>padrões, tendências e fatores de risco,</strong> subsidiando a formulação de políticas públicas.<li>
                    <li>Análise de demanda e consumo de bebidas quentes na planta da Anvisa, utilizando dados históricos e padrões de consumo para subsidiar renegociação contratual,<strong> resultando em maior eficiência econômica e otimização de recursos públicos.</strong><li>
                    <li><strong>Análise transversal do arcabouço legislativo e regulatório da Anvisa,</strong> com abordagem analítica voltada à identificação de impactos normativos, coerência regulatória e apoio à inteligência regulatória.<li>
                    <li><strong>Análise econômico-financeira de contrato de prestação de serviços de transporte executivo,</strong> avaliando custos, utilização e eficiência operacional, o que resultou em revisão estratégica do modelo de contratação e otimização do gasto público.<li>
                    </ul>
                    
               <section>
            <h2>Formação Acadêmica e Idiomas</h2>
            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Ciência de Dados e Inteligência Artificial</span> <span class="sep">|</span> <span class="entry-company">Universidade Oswaldo Cruz</span>
                    </div>
                    <span class="entry-date">Conclusão: 2025</span>
                </div>
            </div>
            <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Inteligência Artificial para Predições em Vigilância e Saúde</span> <span class="sep">|</span> <span class="entry-company">Profep/USP</span>
                    </div>
                    <span class="entry-date">Conclusão: 2025</span>
                </div>

                <div class="entry">
                <div class="entry-header">
                    <div class="entry-title-group">
                        <span class="entry-title">Inglês Intermediário</span> <span class="sep">|</span> <span class="entry-company">Nível B3</span>
                    </div>
                </div>           
            </div>
             </section>
  </body>
</html>

