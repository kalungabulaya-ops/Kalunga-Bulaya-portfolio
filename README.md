<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Kalunga Bulaya Martin | Portfolio</title>

    <meta name="description"
          content="Portfolio professionnel de Kalunga Bulaya Martin - Communication, relations internationales, administration et relation client.">

    <style>
        /* =========================
           RÉGLAGES GÉNÉRAUX
        ========================== */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            color: #1f2937;
            background: #f8fafc;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            width: 90%;
            max-width: 1100px;
            margin: auto;
        }


        /* =========================
           MENU
        ========================== */

        header {
            background: #0f172a;
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            min-height: 70px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
        }

        .logo span {
            color: #38bdf8;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        .nav-links a {
            color: white;
            font-size: 15px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #38bdf8;
        }


        /* =========================
           ACCUEIL
        ========================== */

        .hero {
            min-height: 90vh;
            display: flex;
            align-items: center;
            background: linear-gradient(135deg, #0f172a, #1e3a8a);
            color: white;
        }

        .hero-content {
            display: grid;
            grid-template-columns: 1.4fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero h1 {
            font-size: 52px;
            line-height: 1.1;
            margin: 15px 0;
        }

        .hero h1 span {
            color: #38bdf8;
        }

        .hero-subtitle {
            font-size: 21px;
            color: #dbeafe;
            margin-bottom: 20px;
        }

        .hero-text {
            color: #e2e8f0;
            max-width: 650px;
            margin-bottom: 30px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 13px 22px;
            border-radius: 8px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn-primary {
            background: #38bdf8;
            color: #082f49;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
        }

        .btn-secondary {
            border: 1px solid white;
            color: white;
        }

        .btn-secondary:hover {
            background: white;
            color: #0f172a;
        }


        /* =========================
           PHOTO
        ========================== */

        .profile-photo {
            display: flex;
            justify-content: center;
        }

        .profile-photo img {
            width: 300px;
            height: 300px;
            object-fit: cover;
            border-radius: 50%;
            border: 7px solid rgba(255,255,255,0.2);
        }


        /* =========================
           SECTIONS
        ========================== */

        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 35px;
            color: #0f172a;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #64748b;
        }


        /* =========================
           À PROPOS
        ========================== */

        .about {
            background: white;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text p {
            margin-bottom: 15px;
        }

        .about-info {
            background: #f1f5f9;
            padding: 30px;
            border-radius: 12px;
        }

        .about-info p {
            margin-bottom: 12px;
        }

        .about-info strong {
            color: #0f172a;
        }


        /* =========================
           COMPÉTENCES
        ========================== */

        .skills {
            background: #f8fafc;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .skill {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(15, 23, 42, 0.06);
        }

        .skill h3 {
            margin-bottom: 10px;
            color: #1e3a8a;
        }


        /* =========================
           EXPÉRIENCES
        ========================== */

        .experience {
            background: white;
        }

        .timeline {
            max-width: 850px;
            margin: auto;
        }

        .job {
            border-left: 4px solid #38bdf8;
            padding: 0 0 35px 25px;
            margin-bottom: 25px;
        }

        .job h3 {
            color: #0f172a;
            font-size: 21px;
        }

        .job .company {
            color: #2563eb;
            font-weight: bold;
        }

        .job .date {
            color: #64748b;
            font-size: 14px;
            margin: 5px 0 10px;
        }


        /* =========================
           FORMATION
        ========================== */

        .education {
            background: #f8fafc;
        }

        .education-card {
            max-width: 800px;
            margin: 15px auto;
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(15, 23, 42, 0.05);
        }

        .education-card h3 {
            color: #1e3a8a;
        }


        /* =========================
           PROJETS
        ========================== */

        .projects {
            background: white;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .project-card {
            padding: 25px;
            border: 1px solid #e2e8f0;
            border-radius: 12px;
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(15, 23, 42, 0.08);
        }

        .project-card h3 {
            color: #1e3a8a;
            margin-bottom: 10px;
        }


        /* =========================
           CONTACT
        ========================== */

        .contact {
            background: #0f172a;
            color: white;
        }

        .contact .section-title h2 {
            color: white;
        }

        .contact .section-title p {
            color: #cbd5e1;
        }

        .contact-box {
            max-width: 700px;
            margin: auto;
            text-align: center;
        }

        .contact-box p {
            margin-bottom: 15px;
            color: #e2e8f0;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 25px;
        }

        .contact-link {
            border: 1px solid #475569;
            padding: 12px 20px;
            border-radius: 8px;
            transition: 0.3s;
        }

        .contact-link:hover {
            background: #38bdf8;
            color: #082f49;
        }


        /* =========================
           FOOTER
        ========================== */

        footer {
            background: #020617;
            color: #94a3b8;
            text-align: center;
            padding: 25px;
            font-size: 14px;
        }


        /* =========================
           MOBILE
        ========================== */

        @media (max-width: 768px) {

            .nav-links {
                display: none;
            }

            .hero {
                padding: 70px 0;
            }

            .hero-content {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero h1 {
                font-size: 38px;
            }

            .buttons {
                justify-content: center;
            }

            .profile-photo {
                order: -1;
            }

            .profile-photo img {
                width: 220px;
                height: 220px;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }

            section {
                padding: 60px 0;
            }
        }
    </style>
</head>


<body>

    <!-- =========================
         MENU
    ========================== -->

    <header>
        <nav class="container">

            <div class="logo">
                Martin<span>.</span>
            </div>

            <ul class="nav-links">
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#apropos">À propos</a></li>
                <li><a href="#competences">Compétences</a></li>
                <li><a href="#experiences">Expériences</a></li>
                <li><a href="#formation">Formation</a></li>
                <li><a href="#projets">Projets</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

        </nav>
    </header>


    <!-- =========================
         ACCUEIL
    ========================== -->

    <section class="hero" id="accueil">

        <div class="container hero-content">

            <div>

                <p>Bonjour, je suis</p>

                <h1>
                    Kalunga Bulaya <span>Martin</span>
                </h1>

                <p class="hero-subtitle">
                    Communication • Relations internationales • Administration • Relation client
                </p>

                <p class="hero-text">
                    Professionnel polyvalent, je mets mes compétences en
                    communication, organisation, négociation et gestion
                    administrative au service des organisations et des projets
                    auxquels je contribue.
                </p>

                <div class="buttons">

                    <a href="#apropos" class="btn btn-primary">
                        Découvrir mon parcours
                    </a>

                    <a href="CV_Kalunga_Bulaya_Martin.pdf"
                       class="btn btn-secondary"
                       target="_blank">
                        Télécharger mon CV
                    </a>

                </div>

            </div>


            <div class="profile-photo">

                <!--
                REMPLACE "photo.jpg" PAR LE NOM DE TA PHOTO
                -->

                <img src="photo.jpg"
                     alt="Photo professionnelle de Kalunga Bulaya Martin">

            </div>

        </div>

    </section>


    <!-- =========================
         À PROPOS
    ========================== -->

    <section class="about" id="apropos">

        <div class="container">

            <div class="section-title">

                <h2>À propos de moi</h2>

                <p>Mon parcours et mes objectifs professionnels</p>

            </div>


            <div class="about-content">

                <div class="about-text">

                    <p>
                        Je suis Kalunga Bulaya Martin, titulaire d'une formation
                        en droit et disposant d'expériences dans plusieurs
                        domaines professionnels.
                    </p>

                    <p>
                        Mon parcours m'a permis de développer des compétences
                        en communication, relation client, marketing,
                        administration, organisation et travail en équipe.
                    </p>

                    <p>
                        Je m'intéresse particulièrement aux environnements
                        professionnels multiculturels et aux missions qui
                        nécessitent de la rigueur, de la communication et un
                        bon sens relationnel.
                    </p>

                </div>


                <div class="about-info">

                    <p><strong>Nom :</strong> Kalunga Bulaya Martin</p>

                    <p><strong>Domaines :</strong>
                        Communication, administration,
                        relations internationales, relation client
                    </p>

                    <p><strong>Formation :</strong>
                        Droit privé et judiciaire
                    </p>

                    <p><strong>Localisation :</strong>
                        Lubumbashi, RDC
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         COMPÉTENCES
    ========================== -->

    <section class="skills" id="competences">

        <div class="container">

            <div class="section-title">

                <h2>Mes compétences</h2>

                <p>Des compétences développées à travers mes expériences</p>

            </div>


            <div class="skills-grid">

                <div class="skill">

                    <h3>Communication</h3>

                    <p>
                        Communication professionnelle, rédaction,
                        présentation et transmission d'informations.
                    </p>

                </div>


                <div class="skill">

                    <h3>Négociation</h3>

                    <p>
                        Capacité à échanger avec différents interlocuteurs
                        et à rechercher des solutions adaptées.
                    </p>

                </div>


                <div class="skill">

                    <h3>Relation client</h3>

                    <p>
                        Accueil, écoute, compréhension des besoins et
                        accompagnement des clients.
                    </p>

                </div>


                <div class="skill">

                    <h3>Organisation</h3>

                    <p>
                        Gestion des tâches, suivi des dossiers et
                        coordination des activités.
                    </p>

                </div>


                <div class="skill">

                    <h3>Administration</h3>

                    <p>
                        Gestion documentaire, assistance administrative
                        et traitement des informations.
                    </p>

                </div>


                <div class="skill">

                    <h3>Travail en équipe</h3>

                    <p>
                        Collaboration avec différents profils dans des
                        environnements professionnels variés.
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         EXPÉRIENCES
    ========================== -->

    <section class="experience" id="experiences">

        <div class="container">

            <div class="section-title">

                <h2>Expériences professionnelles</h2>

                <p>Mon parcours professionnel</p>

            </div>


            <div class="timeline">


                <div class="job">

                    <h3>Chargé de communication</h3>

                    <p class="company">
                        Pastorale des jeunes
                    </p>

                    <p class="date">
                        Depuis septembre 2024
                    </p>

                    <p>
                        Participation aux activités de communication,
                        organisation et mobilisation autour des activités.
                    </p>

                </div>


                <div class="job">

                    <h3>Secrétaire particulier DRH / Directeur administratif</h3>

                    <p class="company">
                        Ciel Bleu SARL
                    </p>

                    <p class="date">
                        Avril 2024 – Mai 2026
                    </p>

                    <p>
                        Assistance administrative, organisation,
                        gestion des informations et suivi des activités.
                    </p>

                </div>


                <div class="job">

                    <h3>Marketer permanent</h3>

                    <p class="company">
                        Paymob
                    </p>

                    <p class="date">
                        Mars 2024 – Septembre 2024
                    </p>

                    <p>
                        Promotion des services, communication avec les
                        clients et développement de la relation commerciale.
                    </p>

                </div>


                <div class="job">

                    <h3>Vendeur</h3>

                    <p class="company">
                        SK Supermarché
                    </p>

                    <p class="date">
                        Janvier 2023 – Avril 2023
                    </p>

                    <p>
                        Accueil des clients, présentation des produits,
                        vente et accompagnement.
                    </p>

                </div>


                <div class="job">

                    <h3>Stagiaire</h3>

                    <p class="company">
                        Cabinet d'Avocat APACHO KYEMBE
                    </p>

                    <p class="date">
                        Mai 2023 – Juin 2023
                    </p>

                    <p>
                        Découverte du fonctionnement d'un cabinet juridique
                        et participation aux tâches professionnelles.
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         FORMATION
    ========================== -->

    <section class="education" id="formation">

        <div class="container">

            <div class="section-title">

                <h2>Formation</h2>

                <p>Mon parcours académique</p>

            </div>


            <div class="education-card">

                <h3>
                    Licence en Droit privé et judiciaire
                </h3>

                <p>
                    Université de Lubumbashi
                </p>

                <p>
                    2021 – 2023
                </p>

            </div>


            <div class="education-card">

                <h3>
                    Graduat en Droit général
                </h3>

                <p>
                    2018 – 2021
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         PROJETS
    ========================== -->

    <section class="projects" id="projets">

        <div class="container">

            <div class="section-title">

                <h2>Mes projets</h2>

                <p>Projets et réalisations</p>

            </div>


            <div class="projects-grid">


                <div class="project-card">

                    <h3>Portfolio professionnel</h3>

                    <p>
                        Création de mon portfolio professionnel afin de
                        présenter mon parcours, mes compétences et mes
                        expériences.
                    </p>

                </div>


                <div class="project-card">

                    <h3>Communication</h3>

                    <p>
                        Participation à des activités de communication,
                        mobilisation et organisation d'événements.
                    </p>

                </div>


                <div class="project-card">

                    <h3>Développement professionnel</h3>

                    <p>
                        Développement continu de mes compétences en
                        communication, numérique et gestion professionnelle.
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         CONTACT
    ========================== -->

    <section class="contact" id="contact">

        <div class="container">

            <div class="section-title">

                <h2>Contact</h2>

                <p>Vous souhaitez échanger avec moi ?</p>

            </div>


            <div class="contact-box">

                <p>
                    Je suis disponible pour échanger concernant des
                    opportunités professionnelles, collaborations ou projets.
                </p>


                <div class="contact-links">

                    <!-- REMPLACE L'EMAIL PAR TON VRAI EMAIL -->

                    <a href="mailto:tonemail@example.com"
                       class="contact-link">
                        📧 E-mail
                    </a>


                    <!-- REMPLACE PAR TON PROFIL LINKEDIN -->

                    <a href="#"
                       class="contact-link"
                       target="_blank">
                        💼 LinkedIn
                    </a>

                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         FOOTER
    ========================== -->

    <footer>

        <p>
            © 2026 Kalunga Bulaya Martin — Tous droits réservés.
        </p>

    </footer>


</body>
</html>
