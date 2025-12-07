<!DOCTYPE html>  
<html lang="fr">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>ToB Shop - Style - Tech - Beauté</title>  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <link rel="preconnect" href="https://fonts.googleapis.com">  
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">  
    <style>  
        :root {  
            --primary: #2c3e50;  
            --secondary: #e74c3c;  
            --accent: #3498db;  
            --light: #f8f9fa;  
            --dark: #212529;  
            --gray: #6c757d;  
            --border-radius: 8px;  
            --box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);  
            --transition: all 0.3s ease;  
        }  
  
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
  
        body {  
            font-family: 'Poppins', sans-serif;  
            line-height: 1.6;  
            color: var(--dark);  
            background-color: #f9f9f9;  
        }  
  
        h1, h2, h3, h4 {  
            font-family: 'Montserrat', sans-serif;  
            font-weight: 600;  
            margin-bottom: 1rem;  
        }  
  
        .container {  
            width: 100%;  
            max-width: 1200px;  
            margin: 0 auto;  
            padding: 0 20px;  
        }  
  
        /* Header */  
        header {  
            background-color: white;  
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);  
            position: sticky;  
            top: 0;  
            z-index: 1000;  
        }  
  
        .header-top {  
            background-color: var(--primary);  
            color: white;  
            padding: 10px 0;  
            text-align: center;  
            font-size: 0.9rem;  
        }  
  
        .header-content {  
            display: flex;  
            justify-content: space-between;  
            align-items: center;  
            padding: 20px 0;  
        }  
  
        .logo {  
            font-size: 1.8rem;  
            font-weight: 700;  
            color: var(--primary);  
            display: flex;  
            align-items: center;  
        }  
  
        .logo span {  
            color: var(--secondary);  
        }  
  
        .logo i {  
            margin-right: 10px;  
            font-size: 2rem;  
        }  
  
        .nav-links {  
            display: flex;  
            list-style: none;  
        }  
  
        .nav-links li {  
            margin-left: 30px;  
        }  
  
        .nav-links a {  
            text-decoration: none;  
            color: var(--dark);  
            font-weight: 500;  
            transition: var(--transition);  
        }  
  
        .nav-links a:hover {  
            color: var(--secondary);  
        }  
  
        .header-actions {  
            display: flex;  
            align-items: center;  
        }  
  
        .cart-icon {  
            position: relative;  
            margin-left: 20px;  
            font-size: 1.3rem;  
            color: var(--primary);  
            cursor: pointer;  
        }  
  
        .cart-count {  
            position: absolute;  
            top: -8px;  
            right: -8px;  
            background-color: var(--secondary);  
            color: white;  
            font-size: 0.7rem;  
            width: 18px;  
            height: 18px;  
            border-radius: 50%;  
            display: flex;  
            align-items: center;  
            justify-content: center;  
        }  
  
        .mobile-menu-btn {  
            display: none;  
            font-size: 1.5rem;  
            cursor: pointer;  
            color: var(--primary);  
        }  
  
        /* Hero Section */  
        .hero {  
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1441986300917-64674bd600d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80');  
            background-size: cover;  
            background-position: center;  
            color: white;  
            text-align: center;  
            padding: 100px 0;  
            margin-bottom: 60px;  
        }  
  
        .hero h1 {  
            font-size: 3rem;  
            margin-bottom: 20px;  
        }  
  
        .hero p {  
            font-size: 1.2rem;  
            max-width: 700px;  
            margin: 0 auto 30px;  
            opacity: 0.9;  
        }  
  
        .btn {  
            display: inline-block;  
            background-color: var(--secondary);  
            color: white;  
            padding: 12px 30px;  
            border-radius: var(--border-radius);  
            text-decoration: none;  
            font-weight: 600;  
            border: none;  
            cursor: pointer;  
            transition: var(--transition);  
        }  
  
        .btn:hover {  
            background-color: #c0392b;  
            transform: translateY(-3px);  
            box-shadow: 0 7px 15px rgba(0, 0, 0, 0.1);  
        }  
  
        .btn-outline {  
            background-color: transparent;  
            border: 2px solid white;  
            margin-left: 15px;  
        }  
  
        .btn-outline:hover {  
            background-color: white;  
            color: var(--primary);  
        }  
  
        /* Features Section */  
        .features {  
            padding: 60px 0;  
            background-color: white;  
        }  
  
        .section-title {  
            text-align: center;  
            margin-bottom: 40px;  
            position: relative;  
        }  
  
        .section-title:after {  
            content: '';  
            position: absolute;  
            bottom: -10px;  
            left: 50%;  
            transform: translateX(-50%);  
            width: 80px;  
            height: 4px;  
            background-color: var(--secondary);  
        }  
  
        .features-grid {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
            gap: 30px;  
        }  
  
        .feature-card {  
            background-color: var(--light);  
            padding: 30px;  
            border-radius: var(--border-radius);  
            text-align: center;  
            transition: var(--transition);  
            box-shadow: var(--box-shadow);  
        }  
  
        .feature-card:hover {  
            transform: translateY(-10px);  
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);  
        }  
  
        .feature-card i {  
            font-size: 2.5rem;  
            color: var(--accent);  
            margin-bottom: 20px;  
        }  
  
        .feature-card h3 {  
            font-size: 1.3rem;  
            margin-bottom: 15px;  
        }  
  
        /* Products Section */  
        .products {  
            padding: 60px 0;  
        }  
  
        .category-filter {  
            display: flex;  
            justify-content: center;  
            margin-bottom: 40px;  
            flex-wrap: wrap;  
            gap: 10px;  
        }  
  
        .category-btn {  
            background-color: white;  
            border: 2px solid #e0e0e0;  
            padding: 8px 20px;  
            border-radius: 30px;  
            cursor: pointer;  
            font-weight: 500;  
            transition: var(--transition);  
        }  
  
        .category-btn.active, .category-btn:hover {  
            background-color: var(--secondary);  
            color: white;  
            border-color: var(--secondary);  
        }  
  
        .products-grid {  
            display: grid;  
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));  
            gap: 30px;  
        }  
  
        .product-card {  
            background-color: white;  
            border-radius: var(--border-radius);  
            overflow: hidden;  
            box-shadow: var(--box-shadow);  
            transition: var(--transition);  
        }  
  
        .product-card:hover {  
            transform: translateY(-10px);  
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);  
        }  
  
        .product-image {  
            height: 200px;  
            overflow: hidden;  
        }  
  
        .product-image img {  
            width: 100%;  
            height: 100%;  
            object-fit: cover;  
            transition: var(--transition);  
        }  
  
        .product-card:hover .product-image img {  
            transform: scale(1.05);  
        }  
  
        .product-info {  
            padding: 20px;  
        }  
  
        .product-category {  
            color: var(--gray);  
            font-size: 0.9rem;  
            margin-bottom: 5px;  
        }  
  
        .product-title {  
            font-size: 1.2rem;  
            margin-bottom: 10px;  
            height: 50px;  
            overflow: hidden;  
        }  
  
        .product-price {  
            font-size: 1.5rem;  
            font-weight: 700;  
            color: var(--secondary);  
            margin-bottom: 15px;  
        }  
  
        .product-actions {  
            display: flex;  
            justify-content: space-between;  
        }  
  
        .btn-add-to-cart {  
            background-color: var(--primary);  
            width: 100%;  
            text-align: center;  
        }  
  
        .btn-add-to-cart:hover {  
            background-color: #1a252f;  
        }  
  
        /* Cart Sidebar */  
        .cart-sidebar {  
            position: fixed;  
            top: 0;  
            right: -400px;  
            width: 100%;  
            max-width: 400px;  
            height: 100vh;  
            background-color: white;  
            box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);  
            z-index: 1100;  
            transition: var(--transition);  
            padding: 30px;  
            overflow-y: auto;  
        }  
  
        .cart-sidebar.active {  
            right: 0;  
        }  
  
        .cart-header {  
            display: flex;  
            justify-content: space-between;  
            align-items: center;  
            margin-bottom: 30px;  
            padding-bottom: 15px;  
            border-bottom: 1px solid #eee;  
        }  
  
        .close-cart {  
            background: none;  
            border: none;  
            font-size: 1.5rem;  
            cursor: pointer;  
            color: var(--gray);  
        }  
  
        .cart-items {  
            margin-bottom: 30px;  
        }  
  
        .cart-item {  
            display: flex;  
            margin-bottom: 20px;  
            padding-bottom: 20px;  
            border-bottom: 1px solid #eee;  
        }  
  
        .cart-item-image {  
            width: 80px;  
            height: 80px;  
            border-radius: var(--border-radius);  
            overflow: hidden;  
            margin-right: 15px;  
        }  
  
        .cart-item-image img {  
            width: 100%;  
            height: 100%;  
            object-fit: cover;  
        }  
  
        .cart-item-details {  
            flex: 1;  
        }  
  
        .cart-item-title {  
            font-weight: 600;  
            margin-bottom: 5px;  
        }  
  
        .cart-item-price {  
            color: var(--secondary);  
            font-weight: 600;  
        }  
  
        .cart-item-remove {  
            background: none;  
            border: none;  
            color: var(--gray);  
            cursor: pointer;  
        }  
  
        .cart-total {  
            display: flex;  
            justify-content: space-between;  
            font-size: 1.2rem;  
            font-weight: 700;  
            margin-bottom: 20px;  
            padding-top: 20px;  
            border-top: 2px solid #eee;  
        }  
  
        .overlay {  
            position: fixed;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background-color: rgba(0, 0, 0, 0.5);  
            z-index: 1050;  
            display: none;  
        }  
  
        .overlay.active {  
            display: block;  
        }  
  
        /* Contact Section */  
        .contact {  
            padding: 60px 0;  
            background-color: var(--primary);  
            color: white;  
        }  
  
        .contact-container {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));  
            gap: 40px;  
        }  
  
        .contact-info h3 {  
            color: white;  
            margin-bottom: 20px;  
        }  
  
        .contact-info p {  
            margin-bottom: 10px;  
            opacity: 0.9;  
        }  
  
        .contact-info i {  
            margin-right: 10px;  
            color: var(--accent);  
        }  
  
        .contact-form input, .contact-form textarea {  
            width: 100%;  
            padding: 12px 15px;  
            margin-bottom: 20px;  
            border-radius: var(--border-radius);  
            border: none;  
            font-family: 'Poppins', sans-serif;  
        }  
  
        .contact-form button {  
            background-color: var(--secondary);  
            color: white;  
            border: none;  
        }  
  
        /* Footer */  
        footer {  
            background-color: #1a252f;  
            color: white;  
            padding: 60px 0 20px;  
        }  
  
        .footer-content {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
            gap: 40px;  
            margin-bottom: 40px;  
        }  
  
        .footer-logo {  
            font-size: 1.8rem;  
            font-weight: 700;  
            color: white;  
            margin-bottom: 20px;  
            display: block;  
        }  
  
        .footer-logo span {  
            color: var(--secondary);  
        }  
  
        .footer-links h4 {  
            color: white;  
            margin-bottom: 20px;  
            font-size: 1.2rem;  
        }  
  
        .footer-links ul {  
            list-style: none;  
        }  
  
        .footer-links li {  
            margin-bottom: 10px;  
        }  
  
        .footer-links a {  
            color: #b0b0b0;  
            text-decoration: none;  
            transition: var(--transition);  
        }  
  
        .footer-links a:hover {  
            color: white;  
        }  
  
        .social-links {  
            display: flex;  
            gap: 15px;  
            margin-top: 20px;  
        }  
  
        .social-links a {  
            display: flex;  
            align-items: center;  
            justify-content: center;  
            width: 40px;  
            height: 40px;  
            background-color: rgba(255, 255, 255, 0.1);  
            border-radius: 50%;  
            color: white;  
            transition: var(--transition);  
        }  
  
        .social-links a:hover {  
            background-color: var(--secondary);  
            transform: translateY(-3px);  
        }  
  
        .copyright {  
            text-align: center;  
            padding-top: 20px;  
            border-top: 1px solid rgba(255, 255, 255, 0.1);  
            color: #b0b0b0;  
            font-size: 0.9rem;  
        }  
  
        /* Responsive */  
        @media (max-width: 992px) {  
            .hero h1 {  
                font-size: 2.5rem;  
            }  
        }  
  
        @media (max-width: 768px) {  
            .nav-links, .header-actions .btn {  
                display: none;  
            }  
  
            .mobile-menu-btn {  
                display: block;  
            }  
  
            .hero {  
                padding: 80px 0;  
            }  
  
            .hero h1 {  
                font-size: 2rem;  
            }  
  
            .btn-outline {  
                margin-left: 0;  
                margin-top: 10px;  
                display: block;  
            }  
  
            .header-content {  
                padding: 15px 0;  
            }  
        }  
  
        @media (max-width: 576px) {  
            .cart-sidebar {  
                max-width: 100%;  
            }  
              
            .products-grid {  
                grid-template-columns: 1fr;  
            }  
        }  
    </style>  
</head>  
<body>  
    <!-- Header -->  
    <header>  
        <div class="header-top">  
            <p>Livraison partout à Conakry</p>  
        </div>  
        <div class="container">  
            <div class="header-content">  
                <div class="logo">  
                    <i class="fas fa-store"></i>  
                    ToB<span>Shop</span>  
                </div>  
                <ul class="nav-links">  
                    <li><a href="#home">Accueil</a></li>  
                    <li><a href="#products">Produits</a></li>  
                    <li><a href="#features">Pourquoi nous?</a></li>  
                    <li><a href="#contact">Contact</a></li>  
                </ul>  
                <div class="header-actions">  
                    <a href="#contact" class="btn">Nous contacter</a>  
                    <div class="cart-icon" id="cartIcon">  
                        <i class="fas fa-shopping-cart"></i>  
                        <span class="cart-count">0</span>  
                    </div>  
                </div>  
                <div class="mobile-menu-btn" id="mobileMenuBtn">  
                    <i class="fas fa-bars"></i>  
                </div>  
            </div>  
        </div>  
    </header>  
  
    <!-- Hero Section -->  
    <section class="hero" id="home">  
        <div class="container">  
            <h1>Style - Tech - Beauté</h1>  
            <p>La boutique premium qui mélange élégance, technologie et soins. Découvrez nos produits soigneusement sélectionnés pour votre style et bien-être.</p>  
            <a href="#products" class="btn">Voir la boutique</a>  
            <a href="#contact" class="btn btn-outline">Nous contacter</a>  
        </div>  
    </section>  
  
    <!-- Features Section -->  
    <section class="features" id="features">  
        <div class="container">  
            <h2 class="section-title">Pourquoi choisir Tob Shop ?</h2>  
            <div class="features-grid">  
                <div class="feature-card">  
                    <i class="fas fa-star"></i>  
                    <h3>Produits de qualité sélectionnés</h3>  
                    <p>Nous sélectionnons rigoureusement chaque produit pour vous garantir excellence et durabilité.</p>  
                </div>  
                <div class="feature-card">  
                    <i class="fas fa-tag"></i>  
                    <h3>Prix accessibles</h3>  
                    <p>Des prix compétitifs sans compromis sur la qualité pour rendre le premium accessible à tous.</p>  
                </div>  
                <div class="feature-card">  
                    <i class="fas fa-headset"></i>  
                    <h3>Service client réactif</h3>  
                    <p>Notre équipe est disponible pour répondre à vos questions et résoudre vos problèmes rapidement.</p>  
                </div>  
                <div class="feature-card">  
                    <i class="fas fa-shield-alt"></i>  
                    <h3>Garantie satisfaction</h3>  
                    <p>Nous garantissons votre satisfaction ou vous êtes remboursé sous 14 jours.</p>  
                </div>  
                <div class="feature-card">  
                    <i class="fas fa-shipping-fast"></i>  
                    <h3>Livraison rapide sur Conakry</h3>  
                    <p>Recevez vos commandes en moins de 24h dans toute la ville de Conakry.</p>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Products Section -->  
    <section class="products" id="products">  
        <div class="container">  
            <h2 class="section-title">Nos catégories principales</h2>  
            <div class="category-filter" id="categoryFilter">  
                <button class="category-btn active" data-category="all">Tous les produits</button>  
                <button class="category-btn" data-category="montre">Montres</button>  
                <button class="category-btn" data-category="electronique">Électronique</button>  
                <button class="category-btn" data-category="beaute">Beauté</button>  
                <button class="category-btn" data-category="style">Style</button>  
            </div>  
            <div class="products-grid" id="productsGrid">  
                <!-- Products will be loaded here by JavaScript -->  
            </div>  
        </div>  
    </section>  
  
    <!-- Contact Section -->  
    <section class="contact" id="contact">  
        <div class="container">  
            <h2 class="section-title">Nous contacter</h2>  
            <div class="contact-container">  
                <div class="contact-info">  
                    <h3>Informations de contact</h3>  
                    <p><i class="fas fa-map-marker-alt"></i> Livraison partout à Conakry</p>  
                    <p><i class="fas fa-phone"></i> +224 123 456 789</p>  
                    <p><i class="fas fa-envelope"></i> contact@tobshop.com</p>  
                    <p><i class="fas fa-clock"></i> Lundi - Samedi: 8h00 - 20h00</p>  
                    <div class="social-links">  
                        <a href="#"><i class="fab fa-facebook-f"></i></a>  
                        <a href="#"><i class="fab fa-instagram"></i></a>  
                        <a href="#"><i class="fab fa-whatsapp"></i></a>  
                    </div>  
                </div>  
                <div class="contact-form">  
                    <h3>Envoyez-nous un message</h3>  
                    <form id="contactForm">  
                        <input type="text" placeholder="Votre nom" required>  
                        <input type="email" placeholder="Votre email" required>  
                        <input type="tel" placeholder="Votre téléphone">  
                        <textarea rows="5" placeholder="Votre message" required></textarea>  
                        <button type="submit" class="btn">Envoyer le message</button>  
                    </form>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Footer -->  
    <footer>  
        <div class="container">  
            <div class="footer-content">  
                <div>  
                    <a href="#" class="footer-logo">ToB<span>Shop</span></a>  
                    <p>La boutique premium qui mélange élégance, technologie et soins. Nous nous engageons à vous offrir les meilleurs produits avec un service exceptionnel.</p>  
                </div>  
                <div class="footer-links">  
                    <h4>Liens rapides</h4>  
                    <ul>  
                        <li><a href="#home">Accueil</a></li>  
                        <li><a href="#products">Produits</a></li>  
                        <li><a href="#features">Pourquoi nous?</a></li>  
                        <li><a href="#contact">Contact</a></li>  
                    </ul>  
                </div>  
                <div class="footer-links">  
                    <h4>Catégories</h4>  
                    <ul>  
                        <li><a href="#" data-category="montre">Montres</a></li>  
                        <li><a href="#" data-category="electronique">Électronique</a></li>  
                        <li><a href="#" data-category="beaute">Beauté</a></li>  
                        <li><a href="#" data-category="style">Style</a></li>  
                    </ul>  
                </div>  
                <div class="footer-links">  
                    <h4>Informations</h4>  
                    <ul>  
                        <li><a href="#">Politique de livraison</a></li>  
                        <li><a href="#">Garantie produit</a></li>  
                        <li><a href="#">Méthodes de paiement</a></li>  
                        <li><a href="#">FAQ</a></li>  
                    </ul>  
                </div>  
            </div>  
            <div class="copyright">  
                <p>&copy; 2023 ToB Shop. Tous droits réservés.</p>  
            </div>  
        </div>  
    </footer>  
  
    <!-- Cart Sidebar -->  
    <div class="cart-sidebar" id="cartSidebar">  
        <div class="cart-header">  
            <h3>Votre Panier</h3>  
            <button class="close-cart" id="closeCart">  
                <i class="fas fa-times"></i>  
            </button>  
        </div>  
        <div class="cart-items" id="cartItems">  
            <!-- Cart items will be loaded here -->  
            <p class="empty-cart-message">Votre panier est vide</p>  
        </div>  
        <div class="cart-total">  
            <span>Total:</span>  
            <span id="cartTotal">0 GNF</span>  
        </div>  
        <button class="btn" id="checkoutBtn" style="width: 100%;">Commander maintenant</button>  
    </div>  
    <div class="overlay" id="overlay"></div>  
  
    <script>  
        // Données des produits  
        const products = [  
            {  
                id: 1,  
                title: "Montre élégante chronographe",  
                category: "montre",  
                price: 250000,  
                image: "https://images.unsplash.com/photo-1523170335258-f5ed11844a49?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Montre élégante avec chronographe, bracelet en cuir véritable, étanche jusqu'à 50m."  
            },  
            {  
                id: 2,  
                title: "Casque audio sans fil",  
                category: "electronique",  
                price: 300000,  
                image: "https://images.unsplash.com/photo-1505740420928-5e560c06d30e?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Casque audio sans fil avec réduction de bruit active et autonomie de 30 heures."  
            },  
            {  
                id: 3,  
                title: "Smartphone haut de gamme",  
                category: "electronique",  
                price: 4500000,  
                image: "https://images.unsplash.com/photo-1592899677977-9c10ca588bbd?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Smartphone dernière génération avec écran AMOLED, triple caméra et charge rapide."  
            },  
            {  
                id: 4,  
                title: "Montre connectée sport",  
                category: "montre",  
                price: 350000,  
                image: "https://images.unsplash.com/photo-1579586337278-3fec199a5b6e?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Montre connectée avec suivi d'activités, fréquence cardiaque et notifications."  
            },  
            {  
                id: 5,  
                title: "Kit soin visage premium",  
                category: "beaute",  
                price: 180000,  
                image: "https://images.unsplash.com/photo-1556228578-9c360e1d8d34?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Kit complet de soin visage avec produits naturels pour une peau éclatante."  
            },  
            {  
                id: 6,  
                title: "Sac à main designer",  
                category: "style",  
                price: 550000,  
                image: "https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Sac à main en cuir véritable, design élégant et spacieux pour un usage quotidien."  
            },  
            {  
                id: 7,  
                title: "Parfum signature",  
                category: "beaute",  
                price: 280000,  
                image: "https://images.unsplash.com/photo-1541643600914-78b084683601?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Parfum signature aux notes boisées et florales pour une senteur unique et durable."  
            },  
            {  
                id: 8,  
                title: "Lunettes de soleil polarisées",  
                category: "style",  
                price: 120000,  
                image: "https://images.unsplash.com/photo-1572635196237-14b3f281503f?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80",  
                description: "Lunettes de soleil avec verres polarisés pour une protection optimale contre les UV."  
            }  
        ];  
  
        // Panier  
        let cart = [];  
        const cartCount = document.querySelector('.cart-count');  
        const cartItems = document.getElementById('cartItems');  
        const cartTotal = document.getElementById('cartTotal');  
        const cartIcon = document.getElementById('cartIcon');  
        const cartSidebar = document.getElementById('cartSidebar');  
        const closeCart = document.getElementById('closeCart');  
        const overlay = document.getElementById('overlay');  
        const checkoutBtn = document.getElementById('checkoutBtn');  
        const productsGrid = document.getElementById('productsGrid');  
        const categoryFilter = document.getElementById('categoryFilter');  
        const contactForm = document.getElementById('contactForm');  
  
        // Afficher les produits  
        function displayProducts(filter = 'all') {  
            productsGrid.innerHTML = '';  
              
            const filteredProducts = filter === 'all'   
                ? products   
                : products.filter(product => product.category === filter);  
              
            filteredProducts.forEach(product => {  
                const productCard = document.createElement('div');  
                productCard.className = 'product-card';  
                productCard.innerHTML = `  
                    <div class="product-image">  
                        <img src="${product.image}" alt="${product.title}">  
                    </div>  
                    <div class="product-info">  
                        <div class="product-category">${getCategoryName(product.category)}</div>  
                        <h3 class="product-title">${product.title}</h3>  
                        <p>${product.description}</p>  
                        <div class="product-price">${formatPrice(product.price)} GNF</div>  
                        <div class="product-actions">  
                            <button class="btn btn-add-to-cart" data-id="${product.id}">Ajouter au panier</button>  
                        </div>  
                    </div>  
                `;  
                productsGrid.appendChild(productCard);  
            });  
              
            // Ajouter les événements aux boutons "Ajouter au panier"  
            document.querySelectorAll('.btn-add-to-cart').forEach(button => {  
                button.addEventListener('click', function() {  
                    const productId = parseInt(this.getAttribute('data-id'));  
                    addToCart(productId);  
                });  
            });  
        }  
  
        // Obtenir le nom de la catégorie  
        function getCategoryName(category) {  
            const categoryNames = {  
                'montre': 'Montre',  
                'electronique': 'Électronique',  
                'beaute': 'Beauté',  
                'style': 'Style'  
            };  
            return categoryNames[category] || category;  
        }  
  
        // Formater le prix  
        function formatPrice(price) {  
            return price.toString().replace(/\B(?=(\d{3})+(?!\d))/g, " ");  
        }  
  
        // Ajouter au panier  
        function addToCart(productId) {  
            const product = products.find(p => p.id === productId);  
            const existingItem = cart.find(item => item.id === productId);  
              
            if (existingItem) {  
                existingItem.quantity += 1;  
            } else {  
                cart.push({  
                    ...product,  
                    quantity: 1  
                });  
            }  
              
            updateCart();  
            showNotification(`${product.title} ajouté au panier!`);  
        }  
  
        // Mettre à jour le panier  
        function updateCart() {  
            // Mettre à jour le compteur  
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);  
            cartCount.textContent = totalItems;  
              
            // Mettre à jour la sidebar du panier  
            if (cart.length === 0) {  
                cartItems.innerHTML = '<p class="empty-cart-message">Votre panier est vide</p>';  
                cartTotal.textContent = '0 GNF';  
                checkoutBtn.style.display = 'none';  
            } else {  
                cartItems.innerHTML = '';  
                let total = 0;  
                  
                cart.forEach(item => {  
                    const itemTotal = item.price * item.quantity;  
                    total += itemTotal;  
                      
                    const cartItem = document.createElement('div');  
                    cartItem.className = 'cart-item';  
                    cartItem.innerHTML = `  
                        <div class="cart-item-image">  
                            <img src="${item.image}" alt="${item.title}">  
                        </div>  
                        <div class="cart-item-details">  
                            <h4 class="cart-item-title">${item.title}</h4>  
                            <div class="cart-item-price">${formatPrice(item.price)} GNF</div>  
                            <div style="display: flex; align-items: center; margin-top: 5px;">  
                                <button class="cart-item-decrease" data-id="${item.id}" style="background: #f0f0f0; border: none; width: 25px; height: 25px; border-radius: 50%; cursor: pointer;">-</button>  
                                <span style="margin: 0 10px;">${item.quantity}</span>  
                                <button class="cart-item-increase" data-id="${item.id}" style="background: #f0f0f0; border: none; width: 25px; height: 25px; border-radius: 50%; cursor: pointer;">+</button>  
                                <button class="cart-item-remove" data-id="${item.id}" style="background: none; border: none; color: #e74c3c; margin-left: 15px; cursor: pointer;">  
                                    <i class="fas fa-trash"></i>  
                                </button>  
                            </div>  
                        </div>  
                    `;  
                    cartItems.appendChild(cartItem);  
                });  
                  
                cartTotal.textContent = `${formatPrice(total)} GNF`;  
                checkoutBtn.style.display = 'block';  
                  
                // Ajouter les événements aux boutons du panier  
                document.querySelectorAll('.cart-item-decrease').forEach(button => {  
                    button.addEventListener('click', function() {  
                        const productId = parseInt(this.getAttribute('data-id'));  
                        updateCartItemQuantity(productId, -1);  
                    });  
                });  
                  
                document.querySelectorAll('.cart-item-increase').forEach(button => {  
                    button.addEventListener('click', function() {  
                        const productId = parseInt(this.getAttribute('data-id'));  
                        updateCartItemQuantity(productId, 1);  
                    });  
                });  
                  
                document.querySelectorAll('.cart-item-remove').forEach(button => {  
                    button.addEventListener('click', function() {  
                        const productId = parseInt(this.getAttribute('data-id'));  
                        removeFromCart(productId);  
                    });  
                });  
            }  
        }  
  
        // Mettre à jour la quantité d'un article  
        function updateCartItemQuantity(productId, change) {  
            const item = cart.find(item => item.id === productId);  
              
            if (item) {  
                item.quantity += change;  
                  
                if (item.quantity <= 0) {  
                    cart = cart.filter(item => item.id !== productId);  
                }  
                  
                updateCart();  
            }  
        }  
  
        // Supprimer du panier  
        function removeFromCart(productId) {  
            cart = cart.filter(item => item.id !== productId);  
            updateCart();  
            showNotification('Produit retiré du panier!');  
        }  
  
        // Afficher une notification  
        function showNotification(message) {  
            // Créer l'élément de notification  
            const notification = document.createElement('div');  
            notification.style.cssText = `  
                position: fixed;  
                top: 20px;  
                right: 20px;  
                background-color: #2ecc71;  
                color: white;  
                padding: 15px 20px;  
                border-radius: 8px;  
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);  
                z-index: 2000;  
                transition: all 0.3s ease;  
                transform: translateX(100%);  
                opacity: 0;  
            `;  
            notification.textContent = message;  
            document.body.appendChild(notification);  
              
            // Animer l'entrée  
            setTimeout(() => {  
                notification.style.transform = 'translateX(0)';  
                notification.style.opacity = '1';  
            }, 10);  
              
            // Supprimer après 3 secondes  
            setTimeout(() => {  
                notification.style.transform = 'translateX(100%)';  
                notification.style.opacity = '0';  
                setTimeout(() => {  
                    document.body.removeChild(notification);  
                }, 300);  
            }, 3000);  
        }  
  
        // Ouvrir/fermer le panier  
        cartIcon.addEventListener('click', () => {  
            cartSidebar.classList.add('active');  
            overlay.classList.add('active');  
        });  
  
        closeCart.addEventListener('click', () => {  
            cartSidebar.classList.remove('active');  
            overlay.classList.remove('active');  
        });  
  
        overlay.addEventListener('click', () => {  
            cartSidebar.classList.remove('active');  
            overlay.classList.remove('active');  
        });  
  
        // Commander  
        checkoutBtn.addEventListener('click', () => {  
            if (cart.length === 0) return;  
              
            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);  
            alert(`Merci pour votre commande! Total: ${formatPrice(total)} GNF\nNotre équipe vous contactera pour la livraison.`);  
              
            // Vider le panier  
            cart = [];  
            updateCart();  
              
            // Fermer le panier  
            cartSidebar.classList.remove('active');  
            overlay.classList.remove('active');  
        });  
  
        // Filtrage par catégorie  
        categoryFilter.addEventListener('click', (e) => {  
            if (e.target.classList.contains('category-btn')) {  
                // Mettre à jour les boutons actifs  
                document.querySelectorAll('.category-btn').forEach(btn => {  
                    btn.classList.remove('active');  
                });  
                e.target.classList.add('active');  
                  
                // Filtrer les produits  
                const category = e.target.getAttribute('data-category');  
                displayProducts(category);  
            }  
        });  
  
        // Navigation vers les catégories depuis le footer  
        document.querySelectorAll('.footer-links a[data-category]').forEach(link => {  
            link.addEventListener('click', function(e) {  
                e.preventDefault();  
                const category = this.getAttribute('data-category');  
                  
                // Activer le bouton de catégorie correspondant  
                document.querySelectorAll('.category-btn').forEach(btn => {  
                    btn.classList.remove('active');  
                    if (btn.getAttribute('data-category') === category) {  
                        btn.classList.add('active');  
                    }  
                });  
                  
                // Afficher les produits filtrés  
                displayProducts(category);  
                  
                // Faire défiler jusqu'aux produits  
                document.getElementById('products').scrollIntoView({ behavior: 'smooth' });  
            });  
        });  
  
        // Menu mobile  
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');  
        const navLinks = document.querySelector('.nav-links');  
          
        mobileMenuBtn.addEventListener('click', () => {  
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';  
            if (navLinks.style.display === 'flex') {  
                navLinks.style.position = 'absolute';  
                navLinks.style.top = '100%';  
                navLinks.style.left = '0';  
                navLinks.style.width = '100%';  
                navLinks.style.backgroundColor = 'white';  
                navLinks.style.flexDirection = 'column';  
                navLinks.style.padding = '20px';  
                navLinks.style.boxShadow = '0 10px 15px rgba(0,0,0,0.1)';  
                  
                navLinks.querySelectorAll('li').forEach(li => {  
                    li.style.margin = '10px 0';  
                });  
            }  
        });  
  
        // Gestion du formulaire de contact  
        contactForm.addEventListener('submit', function(e) {  
            e.preventDefault();  
              
            const name = this.querySelector('input[type="text"]').value;  
            const email = this.querySelector('input[type="email"]').value;  
            const phone = this.querySelector('input[type="tel"]').value;  
            const message = this.querySelector('textarea').value;  
              
            // Ici, normalement, on enverrait les données à un serveur  
            // Pour cette démo, on simule juste l'envoi  
            showNotification(`Merci ${name}! Votre message a été envoyé. Nous vous répondrons bientôt.`);  
            this.reset();  
        });  
  
        // Navigation fluide  
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {  
            anchor.addEventListener('click', function(e) {  
                e.preventDefault();  
                  
                const targetId = this.getAttribute('href');  
                if (targetId === '#') return;  
                  
                const targetElement = document.querySelector(targetId);  
                if (targetElement) {  
                    targetElement.scrollIntoView({  
                        behavior: 'smooth'  
                    });  
                      
                    // Fermer le menu mobile si ouvert  
                    if (window.innerWidth <= 768) {  
                        navLinks.style.display = 'none';  
                    }  
                }  
            });  
        });  
  
        // Initialiser l'affichage des produits  
        displayProducts();  
        updateCart();  
    </script>  
</body>  
</html>  
