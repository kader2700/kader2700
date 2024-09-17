<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ouhod Voyage</title>
    <style>
        /* Ajoutez ici des styles CSS de base */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #3498db;
            color: white;
            padding: 20px;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin-right: 10px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
        }
        .destination-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        .destination-card {
            background-color: white;
            border-radius: 8px;
            padding: 15px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        /* Nouveaux styles */
        form {
            display: flex;
            flex-direction: column;
            max-width: 500px;
            margin: 0 auto;
        }
        form input, form textarea, form select {
            margin-bottom: 15px;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        form button {
            background-color: #3498db;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        form button:hover {
            background-color: #2980b9;
        }
        
        /* Nouveaux styles */
        .offre {
            background-color: #ecf0f1;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
        }
        .prix {
            font-weight: bold;
            color: #e74c3c;
        }
        .offre button {
            background-color: #2ecc71;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
        }
        .offre button:hover {
            background-color: #27ae60;
        }
        footer {
            background-color: #34495e;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Site pour Ouhod Voyage</h1>
        <nav>
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#destinations">Destinations</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="accueil">
            <h2>Bienvenue chez Ouhod Voyage</h2>
            <video width="100%" height="auto" controls>
                <source src="path/to/tourism_video.mp4" type="video/mp4">
                Votre navigateur ne prend pas en charge la balise vidéo.
            </video>
            <p>Découvrez des destinations uniques et vivez des expériences inoubliables avec Ouhod Voyage.</p>
        </section>

        <section id="destinations">
            <h2>Nos Destinations</h2>
            <div class="destination-grid">
                <div class="destination-card">
                    <h3>Paris</h3>
                    <img src="path/to/paris.jpg" alt="Paris" width="100%">
                    <p>Découvrez la ville de l'amour et ses monuments emblématiques.</p>
                </div>
                <div class="destination-card">
                    <h3>Marrakech</h3>
                    <img src="path/to/marrakech.jpg" alt="Marrakech" width="100%">
                    <p>Plongez dans l'atmosphère envoûtante des souks et des palais.</p>
                </div>
                <!-- Nouvelle destination -->
                <div class="destination-card">
                    <h3>Istanbul</h3>
                    <img src="path/to/istanbul.jpg" alt="Istanbul" width="100%">
                    <p>Explorez la ville où l'Orient rencontre l'Occident.</p>
                </div>
                <!-- Ajoutez d'autres destinations selon vos offres -->
            </div>
        </section>

        <section id="services">
            <h2>Nos Services</h2>
            <ul>
                <li>Réservation de vols</li>
                <li>Hébergement de luxe</li>
                <li>Visites guidées personnalisées</li>
                <li>Location de voitures</li>
            </ul>
        </section>

        <section id="contact">
            <h2>Contactez-nous</h2>
            <form>
                <label for="name">Nom :</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email :</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message :</label>
                <textarea id="message" name="message" required></textarea>

                <label for="subject">Sujet :</label>
                <select id="subject" name="subject" required>
                    <option value="">Choisissez un sujet</option>
                    <option value="reservation">Réservation</option>
                    <option value="information">Demande d'information</option>
                    <option value="reclamation">Réclamation</option>
                </select>

                <button type="submit">Envoyer</button>
            </form>
        </section>
    </main>

    <section id="offres-speciales">
        <h2>Offres Spéciales</h2>
        <div class="offre">
            <h3>Séjour de luxe à Bali</h3>
            <p>Profitez de 7 nuits dans un resort 5 étoiles avec petit-déjeuner inclus.</p>
            <p class="prix">À partir de 1299€ par personne</p>
            <button>Réserver maintenant</button>
        </div>
        <div class="offre">
            <h3>Week-end à Rome</h3>
            <p>3 jours / 2 nuits dans un hôtel au cœur de la ville éternelle.</p>
            <p class="prix">À partir de 499€ par personne</p>
            <button>Réserver maintenant</button>
        </div>
    </section>

    <section id="temoignages">
        <h2>Témoignages de nos clients</h2>
        <div class="temoignage">
            <p>"Une expérience inoubliable avec Ouhod Voyage. Tout était parfaitement organisé !"</p>
            <p><strong>- Marie D.</strong></p>
        </div>
        <div class="temoignage">
            <p>"Je recommande vivement leurs services. Des destinations magnifiques et un personnel attentionné."</p>
            <p><strong>- Pierre L.</strong></p>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 Ouhod Voyage. Tous droits réservés.</p>
        <nav>
            <a href="#">Mentions légales</a> |
            <a href="#">Politique de confidentialité</a> |
            <a href="#">Conditions générales de vente</a>
        </nav>
        <p>Suivez-nous sur les réseaux sociaux :</p>
        <a href="#">Facebook</a> |
        <a href="#">Instagram</a> |
        <a href="#">Twitter</a>
    </footer>

    <script>
        // Ajout d'un petit script pour améliorer l'interactivité
        document.querySelectorAll('button').forEach(button => {
            button.addEventListener('click', function() {
                alert('Merci de votre intérêt ! Un conseiller va vous contacter prochainement.');
            });
        });
    </script>
</body>
</html>
