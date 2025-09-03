<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Gustavo R. Colombo - Gestor em Saúde com mais de 10 anos de experiência em direção hospitalar, planejamento estratégico, gestão de projetos e mentoria.">
    <meta name="keywords" content="Gestor de Saúde, Administração Hospitalar, Saúde Pública, Gustavo R. Colombo, Compliance, Acreditação ONA, PMO Saúde, Mentoria em Saúde">
    <title>Gustavo R. Colombo | Gestor em Saúde Pública e Privada</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Montserrat:wght@600;700&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

    <style>
        :root {
            --bg-color: #111827; /* Cinza-azulado muito escuro */
            --primary-color: #1F2937; /* Cinza-azulado escuro para cards */
            --secondary-color: #374151; /* Cinza para bordas e detalhes */
            --text-color: #D1D5DB; /* Cinza claro para texto */
            --highlight-color: #FFFFFF; /* Branco para títulos principais */
            --accent-color: #3B82F6; /* Azul sóbrio para destaque */
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.7;
            font-weight: 300;
        }
        .container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }
        h1, h2, h3 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: var(--highlight-color);
            margin-bottom: 20px;
        }
        h2 { text-align: center; font-size: 2.5rem; margin-bottom: 40px; }
        p { text-align: justify; margin-bottom: 15px; }
        section { padding: 100px 0; }
        .header {
            background-color: rgba(17, 24, 39, 0.8);
            backdrop-filter: blur(10px);
            padding: 20px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--secondary-color);
        }
        .navbar { display: flex; justify-content: space-between; align-items: center; }
        .nav-logo { font-family: 'Montserrat', sans-serif; font-size: 1.5em; font-weight: 600; color: var(--highlight-color); text-decoration: none; }
        .nav-menu { list-style: none; display: flex; gap: 30px; }
        .nav-link { text-decoration: none; color: var(--text-color); font-weight: 400; transition: color 0.3s ease; }
        .nav-link:hover { color: var(--accent-color); }
        .hamburger { display: none; }
        .bar { display: block; width: 25px; height: 3px; margin: 5px auto; transition: all 0.3s ease-in-out; background-color: var(--highlight-color); }
        .hero {
            background: linear-gradient(rgba(17, 24, 39, 0.7), rgba(17, 24, 39, 0.7)), url('https://images.unsplash.com/photo-1538947151249-38142d191a4e?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4-0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D') center center/cover no-repeat;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }
        .hero-content { max-width: 800px; }
        .hero h1 { font-size: 3.2rem; margin-bottom: 20px; }
        .hero p { font-size: 1.2rem; margin-bottom: 30px; text-align: center; font-weight: 300; }
        .btn { display: inline-block; background-color: var(--accent-color); color: var(--highlight-color); padding: 15px 35px; text-decoration: none; font-weight: 700; border-radius: 5px; transition: background-color 0.3s ease, transform 0.2s ease; }
        .btn:hover { background-color: #2563EB; transform: translateY(-2px); }
        #about .container { display: flex; gap: 60px; align-items: center; }
        .about-text { flex: 2; }
        .about-image { flex: 1; text-align: center; }
        .about-image img {
            max-width: 280px;
            width: 100%;
            border-radius: 50%;
            border: 5px solid var(--secondary-color);
            filter: grayscale(30%) contrast(110%);
        }
        #services { background-color: var(--primary-color); }
        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 40px; }
        .service-card {
            background-color: var(--bg-color);
            padding: 40px 30px;
            border-radius: 8px;
            border-top: 4px solid var(--accent-color);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: flex;
            flex-direction: column;
        }
        .service-card p { text-align: left; font-size: 0.95rem; }
        .service-card:hover { transform: translateY(-8px); box-shadow: 0 10px 20px rgba(0,0,0,0.3); }
        .service-card .icon { font-size: 2.5rem; color: var(--accent-color); margin-bottom: 20px; }
        .service-card h3 { margin-bottom: 15px; font-size: 1.25rem; }
        .contact-container { max-width: 700px; margin: 0 auto; text-align: center; }
        .contact-container p { font-size: 1.1rem; margin-bottom: 20px; text-align: center; }
        .contact-info-item {
            font-size: 1.1rem;
            margin-bottom: 25px;
        }
        .social-icons { list-style: none; padding: 0; display: flex; justify-content: center; gap: 40px; margin-top: 30px; }
        .social-icons a { color: var(--text-color); font-size: 2.5rem; transition: color 0.3s ease, transform 0.2s ease; }
        .social-icons a:hover { color: var(--accent-color); transform: translateY(-3px); }
        .footer { background-color: #000; color: #888; text-align: center; padding: 25px 0; border-top: 1px solid var(--secondary-color); }
        @media (max-width: 768px) {
            h2 { font-size: 2rem; }
            .hero h1 { font-size: 2.5rem; }
            .nav-menu { position: fixed; left: -100%; top: 80px; flex-direction: column; background-color: var(--primary-color); width: 100%; text-align: center; transition: 0.3s; box-shadow: 0 10px 27px rgba(0, 0, 0, 0.05); }
            .nav-menu.active { left: 0; }
            .nav-item { margin: 2rem 0; }
            .hamburger { display: block; cursor: pointer; }
            .hamburger.active .bar:nth-child(2) { opacity: 0; }
            .hamburger.active .bar:nth-child(1) { transform: translateY(8px) rotate(45deg); }
            .hamburger.active .bar:nth-child(3) { transform: translateY(-8px) rotate(-45deg); }
            #about .container { flex-direction: column-reverse; }
        }
    </style>
</head>
<body>

    <header class="header">
        <nav class="navbar container">
            <a href="#home" class="nav-logo">Gustavo R. Colombo</a>
            <ul class="nav-menu">
                <li class="nav-item"><a href="#home" class="nav-link">Início</a></li>
                <li class="nav-item"><a href="#about" class="nav-link">Sobre Mim</a></li>
                <li class="nav-item"><a href="#services" class="nav-link">Áreas de Atuação</a></li>
                <li class="nav-item"><a href="#contact" class="nav-link">Contato</a></li>
            </ul>
            <div class="hamburger">
                <span class="bar"></span><span class="bar"></span><span class="bar"></span>
            </div>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content container">
            <h1>Liderança e Estratégia na Gestão da Saúde</h1>
            <p>Mais de uma década de experiência em direção hospitalar, planejamento estratégico em saúde pública, gestão de projetos e mentoria para otimizar resultados e qualificar o atendimento.</p>
            <a href="#about" class="btn">Conheça Minha Trajetória</a>
        </div>
    </section>

    <section id="about">
        <div class="container">
            <div class="about-text">
                <h2>Gustavo R. Colombo</h2>
                <p>Sou Gestor em Saúde, Bacharel em Administração e Sanitarista, com mais de dez anos de experiência dedicados a liderar e aprimorar organizações de saúde, tanto no setor público quanto no privado. Minha carreira foi construída através da atuação direta em posições estratégicas, desde a coordenação de Unidades Básicas de Saúde até a direção de Hospitais e UPAs, além da Superintendência em Secretarias Municipais de Saúde.</p>
                <p>Com um perfil orientado para resultados e processos, possuo múltiplas especializações, incluindo Administração Hospitalar, Saúde Pública, Compliance e Gestão de Riscos. Atuo como Gerente Corporativo de Projetos (PMO) e Expansão em Organização Social, consolidando uma visão sistêmica que integra planejamento, implantação e operação. Sou também Avaliador do Sistema Brasileiro de Acreditação (ONA), Conselheiro Municipal de Saúde (Caxias do Sul/RS) e membro do Núcleo de Saúde do CRA-SC, participando ativamente do desenvolvimento do setor e oferecendo mentoria para novos líderes e profissionais da área.</p>
            </div>
            <div class="about-image">
                <img src="https://storage.googleapis.com/maker-studio-project-media-prod/11059902640243171328/images/df821217-fe42-4f36-932c-352ca40f2ac7.jpeg" alt="Foto de Gustavo R. Colombo">
            </div>
        </div>
    </section>

    <section id="services">
        <div class="container">
            <h2>Principais Competências e Serviços</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="icon"><i class="fas fa-hospital-user"></i></div>
                    <h3>Gestão de Unidades de Saúde</h3>
                    <p>Direção e administração de hospitais, Unidades de Pronto Atendimento (UPAs), policlínicas e Unidades Básicas de Saúde (UBS), com foco na eficiência operacional, qualidade assistencial e sustentabilidade financeira.</p>
                </div>
                <div class="service-card">
                    <div class="icon"><i class="fas fa-tasks"></i></div>
                    <h3>Planejamento Estratégico em Saúde</h3>
                    <p>Elaboração e execução de planos estratégicos para Secretarias de Saúde e instituições privadas. Definição de metas, indicadores (KPIs) e otimização de fluxos para maximizar o impacto dos recursos.</p>
                </div>
                <div class="service-card">
                    <div class="icon"><i class="fas fa-project-diagram"></i></div>
                    <h3>Implantação de Projetos e PMO</h3>
                    <p>Gerenciamento de projetos complexos na área da saúde, desde a concepção e análise de viabilidade até a implantação e operação. Estruturação de Escritórios de Projetos (PMO) para padronização e controle.</p>
                </div>
                 <div class="service-card">
                    <div class="icon"><i class="fas fa-shield-check"></i></div>
                    <h3>Compliance, Riscos e Acreditação ONA</h3>
                    <p>Implementação de programas de compliance e gestão de riscos. Assessoria para processos de certificação e acreditação de serviços de saúde, utilizando a metodologia do Sistema Brasileiro de Acreditação (ONA).</p>
                </div>
                <div class="service-card">
                    <div class="icon"><i class="fas fa-chalkboard-teacher"></i></div>
                    <h3>Mentoria e Desenvolvimento de Lideranças</h3>
                    <p>Orientação e desenvolvimento de profissionais e futuras lideranças na área da saúde. Compartilhamento de experiência e conhecimentos práticos para impulsionar carreiras e aprimorar a gestão de equipes e unidades.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="contact">
        <div class="container contact-container">
            <h2>Contato</h2>
            <p>Se sua instituição de saúde busca aprimorar a gestão, otimizar processos ou desenvolver novos projetos, estou à disposição para uma conversa.</p>
            
            <div class="contact-info-item">
                <strong>E-mail:</strong> gucolombo@gmail.com
            </div>
            <div class="contact-info-item">
                <strong>Telefone / WhatsApp:</strong> (48) 98453-2543
            </div>

            <ul class="social-icons">
                <li><a href="https://wa.me/5548984532543" target="_blank" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a></li>
                <li><a href="https://www.linkedin.com/in/gustavo-colombo-1053b45b/" target="_blank" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a></li>
                <li><a href="https://www.instagram.com/ogucolombo/" target="_blank" aria-label="Instagram"><i class="fab fa-instagram"></i></a></li>
            </ul>
        </div>
    </section>

    <footer class="footer">
        <p>&copy; 2025 Gustavo R. Colombo. CRA-SC 41.205 / CRA-RS 0060935</p>
    </footer>

    <script>
        const hamburger = document.querySelector(".hamburger");
        const navMenu = document.querySelector(".nav-menu");
        hamburger.addEventListener("click", () => {
            hamburger.classList.toggle("active");
            navMenu.classList.toggle("active");
        });
        document.querySelectorAll(".nav-link").forEach(n => n.addEventListener("click", () => {
            hamburger.classList.remove("active");
            navMenu.classList.remove("active");
        }));
    </script>
</body>
</html>
