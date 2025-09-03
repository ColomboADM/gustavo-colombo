<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Gustavo Colombo - Consultoria especializada em otimização de processos, gestão de produção e planejamento estratégico.">
    <meta name="keywords" content="Consultoria, Engenharia de Produção, Gestão Estratégica, Gustavo Colombo, Otimização de Processos, Indústria 4.0">
    <title>Gustavo Colombo | Consultoria Estratégica em Engenharia e Gestão</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">

    <style>
        /* --- Reset & Base Styles --- */
        :root {
            --bg-color: #121212;
            --primary-color: #1f1f1f;
            --secondary-color: #2a2a2a;
            --text-color: #e0e0e0;
            --highlight-color: #ffffff;
            --accent-color: #4CAF50; /* Um verde sóbrio como cor de destaque */
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        h1, h2, h3 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: var(--highlight-color);
            margin-bottom: 20px;
        }
        
        section {
            padding: 80px 0;
        }

        /* --- Header & Navigation --- */
        .header {
            background-color: rgba(18, 18, 18, 0.8);
            backdrop-filter: blur(10px);
            padding: 20px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--secondary-color);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-logo {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.5em;
            font-weight: 700;
            color: var(--highlight-color);
            text-decoration: none;
        }

        .nav-menu {
            list-style: none;
            display: flex;
            gap: 30px;
        }

        .nav-link {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 600;
            transition: color 0.3s ease;
        }

        .nav-link:hover {
            color: var(--accent-color);
        }
        
        /* Mobile Menu */
        .hamburger {
            display: none;
            cursor: pointer;
        }

        .bar {
            display: block;
            width: 25px;
            height: 3px;
            margin: 5px auto;
            -webkit-transition: all 0.3s ease-in-out;
            transition: all 0.3s ease-in-out;
            background-color: var(--highlight-color);
        }


        /* --- Hero Section --- */
        .hero {
            background: linear-gradient(rgba(18, 18, 18, 0.7), rgba(18, 18, 18, 0.7)), url('https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80') center center/cover no-repeat;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent-color);
            color: var(--highlight-color);
            padding: 15px 30px;
            text-decoration: none;
            font-weight: 700;
            border-radius: 5px;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }
        
        .btn:hover {
            background-color: #45a049;
            transform: translateY(-2px);
        }

        /* --- About Section --- */
        #about {
            background-color: var(--primary-color);
        }
        .about-content {
            display: flex;
            gap: 50px;
            align-items: center;
        }
        .about-text {
            flex: 2;
        }
        .about-image {
            flex: 1;
            text-align: center;
        }
        .about-image img {
            max-width: 300px;
            border-radius: 50%;
            border: 5px solid var(--secondary-color);
        }

        /* --- Services Section --- */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .service-card {
            background-color: var(--primary-color);
            padding: 30px;
            border-radius: 8px;
            border-left: 5px solid var(--accent-color);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        .service-card .icon {
            font-size: 2.5rem;
            color: var(--accent-color);
            margin-bottom: 20px;
        }

        /* --- Publications Section --- */
        #publications {
            background-color: var(--primary-color);
        }

        .publication-item {
            background-color: var(--secondary-color);
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 5px;
        }

        .publication-item strong {
            color: var(--highlight-color);
            display: block;
        }

        .publication-item em {
            font-size: 0.9em;
        }
        
        .center-btn {
            text-align: center;
            margin-top: 40px;
        }


        /* --- Contact Section --- */
        .contact-info {
            margin-top: 40px;
            text-align: center;
        }

        .contact-info p {
            font-size: 1.1rem;
            margin-bottom: 20px;
        }

        .social-icons {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            gap: 30px;
        }

        .social-icons a {
            color: var(--text-color);
            font-size: 2rem;
            transition: color 0.3s ease, transform 0.2s ease;
        }

        .social-icons a:hover {
            color: var(--accent-color);
            transform: translateY(-3px);
        }

        /* --- Footer --- */
        .footer {
            background-color: #0a0a0a;
            color: #888;
            text-align: center;
            padding: 20px 0;
            border-top: 1px solid var(--secondary-color);
        }
        
        /* --- Responsive Design --- */
        @media (max-width: 768px) {
            .nav-menu {
                position: fixed;
                left: -100%;
                top: 80px;
                flex-direction: column;
                background-color: var(--primary-color);
                width: 100%;
                text-align: center;
                transition: 0.3s;
                box-shadow: 0 10px 27px rgba(0, 0, 0, 0.05);
            }

            .nav-menu.active {
                left: 0;
            }

            .nav-item {
                margin: 2.5rem 0;
            }

            .hamburger {
                display: block;
            }
            
            .hamburger.active .bar:nth-child(2) {
                opacity: 0;
            }

            .hamburger.active .bar:nth-child(1) {
                transform: translateY(8px) rotate(45deg);
            }

            .hamburger.active .bar:nth-child(3) {
                transform: translateY(-8px) rotate(-45deg);
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .about-content {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <header class="header">
        <nav class="navbar container">
            <a href="#home" class="nav-logo">Gustavo Colombo</a>
            <ul class="nav-menu">
                <li class="nav-item"><a href="#home" class="nav-link">Início</a></li>
                <li class="nav-item"><a href="#about" class="nav-link">Sobre Mim</a></li>
                <li class="nav-item"><a href="#services" class="nav-link">Serviços</a></li>
                <li class="nav-item"><a href="#publications" class="nav-link">Publicações</a></li>
                <li class="nav-item"><a href="#contact" class="nav
