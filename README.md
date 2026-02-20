:root {
    --primary-gold: #C9A961;
    --dark-bg: #1a1a1a;
    --navy: #2B3E50;
    --light-gray: #f5f5f5;
    --text-dark: #333;
    --text-light: #666;
    --white: #ffffff;
    --accent: #1e3a5f;
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
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-dark);
    overflow-x: hidden;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header */
.header-top {
    background: var(--navy);
    color: var(--white);
    padding: 0.8rem 0;
    font-size: 0.9rem;
}

.header-top .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.contact-bar {
    display: flex;
    gap: 2rem;
}

.contact-bar span {
    display: flex;
    align-items: center;
    gap: 0.5rem;
}

.social-icons {
    display: flex;
    gap: 1rem;
}

.social-icons a {
    color: var(--primary-gold);
    text-decoration: none;
    transition: color 0.3s;
}

.social-icons a:hover {
    color: var(--white);
}

/* Navbar */
.navbar {
    background: var(--white);
    padding: 1rem 0;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

.navbar-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo-section {
    display: flex;
    align-items: center;
    gap: 1rem;
}

.logo {
    height: 50px;
    width: auto;
}

.logo-text h1 {
    font-size: 1.2rem;
    color: var(--navy);
    margin: 0;
}

.logo-text p {
    font-size: 0.8rem;
    color: var(--primary-gold);
    margin: 0;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-menu a {
    color: var(--text-dark);
    text-decoration: none;
    transition: color 0.3s;
    font-weight: 500;
}

.nav-menu a:hover {
    color: var(--primary-gold);
}

.free-consultation-btn {
    background: var(--primary-gold);
    color: var(--navy);
    border: none;
    padding: 0.8rem 1.5rem;
    border-radius: 25px;
    cursor: pointer;
    font-weight: bold;
    transition: all 0.3s;
}

.free-consultation-btn:hover {
    background: #e0c878;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(201, 169, 97, 0.3);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--navy) 0%, var(--accent) 100%);
    color: var(--white);
    padding: 5rem 0;
    min-height: 650px;
    display: flex;
    align-items: center;
}

.hero-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
}

.hero-label {
    display: inline-block;
    background: var(--primary-gold);
    color: var(--navy);
    padding: 0.5rem 1rem;
    border-radius: 25px;
    font-size: 0.85rem;
    font-weight: bold;
    margin-bottom: 1rem;
}

.hero-text h1 {
    font-size: 3.5rem;
    line-height: 1.1;
    margin-bottom: 1.5rem;
}

.hero-text p {
    font-size: 1.1rem;
    margin-bottom: 2rem;
    opacity: 0.95;
}

.hero-buttons {
    display: flex;
    gap: 1rem;
}

.btn {
    padding: 1rem 2rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    font-weight: bold;
    transition: all 0.3s;
    text-decoration: none;
    display: inline-block;
}

.btn-primary {
    background: var(--primary-gold);
    color: var(--navy);
}

.btn-primary:hover {
    background: #e0c878;
    transform: translateY(-2px);
    box-shadow: 0 10px 25px rgba(201, 169, 97, 0.4);
}

.btn-secondary {
    background: transparent;
    color: var(--white);
    border: 2px solid var(--white);
}

.btn-secondary:hover {
    background: var(--white);
    color: var(--navy);
}

.hero-image {
    position: relative;
}

.portrait-image {
    width: 100%;
    border-radius: 10px;
    box-shadow: 0 20px 40px rgba(0,0,0,0.3);
}

/* About Section */
.about {
    padding: 5rem 0;
    background: var(--light-gray);
}

.about-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
}

.about-images {
    position: relative;
}

.image-card {
    position: relative;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 15px 35px rgba(0,0,0,0.15);
}

.image-card img {
    width: 100%;
    display: block;
}

.logo-badge {
    position: absolute;
    bottom: -20px;
    right: -20px;
    width: 120px;
    height: 120px;
    background: var(--white);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

.badge-logo {
    width: 80%;
    height: 80%;
    object-fit: contain;
}

.section-label {
    display: inline-block;
    color: var(--primary-gold);
    font-weight: bold;
    font-size: 0.9rem;
    text-transform: uppercase;
    margin-bottom: 1rem;
    letter-spacing: 1px;
}

.about-text h2 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
    color: var(--navy);
    line-height: 1.2;
}

.about-text p {
    color: var(--text-light);
    margin-bottom: 2rem;
    font-size: 1.05rem;
}

.about-features {
    list-style: none;
    margin-bottom: 2rem;
}

.about-features li {
    display: flex;
    gap: 1rem;
    margin-bottom: 1.5rem;
}

.about-features i {
    color: var(--primary-gold);
    font-size: 1.5rem;
    flex-shrink: 0;
    margin-top: 0.3rem;
}

.about-features h4 {
    color: var(--navy);
    margin-bottom: 0.3rem;
}

.about-features p {
    font-size: 0.95rem;
    margin: 0;
    color: var(--text-light);
}

/* Work Process Section */
.work-process {
    padding: 5rem 0;
    background: var(--dark-bg);
    color: var(--white);
}

.process-header {
    text-align: center;
    margin-bottom: 3rem;
}

.process-header h2 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.process-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}

.process-card {
    background: rgba(201, 169, 97, 0.1);
    padding: 2.5rem;
    border-radius: 10px;
    text-align: center;
    border: 1px solid var(--primary-gold);
    transition: all 0.3s;
}

.process-card:hover {
    background: rgba(201, 169, 97, 0.2);
    transform: translateY(-5px);
}

.process-icon {
    width: 80px;
    height: 80px;
    background: var(--primary-gold);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 1.5rem;
    font-size: 2rem;
    color: var(--navy);
}

.process-card h3 {
    font-size: 1.3rem;
    margin-bottom: 1rem;
}

.process-card p {
    color: rgba(255,255,255,0.8);
    font-size: 0.95rem;
}

/* Services Section */
.services {
    padding: 5rem 0;
    background: var(--white);
}

.services-header {
    text-align: center;
    margin-bottom: 3rem;
}

.services-header h2 {
    font-size: 2.5rem;
    color: var(--navy);
    margin-bottom: 1rem;
}

.services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
    gap: 2rem;
}

.service-card {
    background: var(--white);
    border: 1px solid #e0e0e0;
    padding: 2rem;
    border-radius: 10px;
    text-align: center;
    transition: all 0.3s;
    box-shadow: 0 5px 15px rgba(0,0,0,0.08);
}

.service-card:hover {
    box-shadow: 0 15px 35px rgba(0,0,0,0.15);
    transform: translateY(-5px);
}

.service-card.featured {
    background: var(--primary-gold);
    color: var(--white);
    border: none;
}

.service-card.featured:hover {
    background: #e0c878;
}

.service-icon {
    width: 80px;
    height: 80px;
    background: var(--primary-gold);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 1.5rem;
    font-size: 2rem;
    color: var(--navy);
}

.service-card.featured .service-icon {
    background: var(--navy);
    color: var(--primary-gold);
}

.service-card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: var(--navy);
}

.service-card.featured h3 {
    color: var(--white);
}

.service-card p {
    color: var(--text-light);
    margin-bottom: 1.5rem;
    font-size: 0.95rem;
}

.service-card.featured p {
    color: rgba(255,255,255,0.95);
}

.read-more {
    color: var(--primary-gold);
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

.read-more:hover {
    color: var(--navy);
}

.service-card.featured .read-more {
    color: var(--navy);
}

/* Contact Section */
.contact {
    padding: 5rem 0;
    background: var(--light-gray);
}

.contact h2 {
    text-align: center;
    font-size: 2.5rem;
    color: var(--navy);
    margin-bottom: 3rem;
}

.contact-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
}

.contact-info {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.contact-item {
    display: flex;
    gap: 1.5rem;
}

.contact-icon {
    width: 60px;
    height: 60px;
    background: var(--primary-gold);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    color: var(--navy);
    flex-shrink: 0;
}

.contact-details h3 {
    color: var(--navy);
    margin-bottom: 0.5rem;
}

.contact-details p {
    color: var(--text-light);
}

.contact-details a {
    color: var(--primary-gold);
    text-decoration: none;
}

.contact-details a:hover {
    text-decoration: underline;
}

.contact-form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.contact-form input,
.contact-form textarea {
    padding: 1rem;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-family: inherit;
    font-size: 1rem;
    background: var(--white);
}

.contact-form input:focus,
.contact-form textarea:focus {
    outline: none;
    border-color: var(--primary-gold);
    box-shadow: 0 0 8px rgba(201, 169, 97, 0.3);
}

/* Footer */
.footer {
    background: var(--navy);
    color: var(--white);
    padding: 3rem 0 1rem;
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-bottom: 2rem;
}

.footer-section h3 {
    color: var(--primary-gold);
    margin-bottom: 1rem;
}

.footer-section p {
    color: rgba(255,255,255,0.8);
    font-size: 0.95rem;
}

.footer-section ul {
    list-style: none;
}

.footer-section ul li {
    margin-bottom: 0.5rem;
}

.footer-section a {
    color: rgba(255,255,255,0.8);
    text-decoration: none;
    transition: color 0.3s;
}

.footer-section a:hover {
    color: var(--primary-gold);
}

.footer-bottom {
    border-top: 1px solid rgba(201, 169, 97, 0.3);
    padding-top: 1rem;
    text-align: center;
    color: rgba(255,255,255,0.7);
}

/* Responsive Design */
@media (max-width: 768px) {
    .header-top .container {
        flex-direction: column;
        gap: 1rem;
        text-align: center;
    }

    .contact-bar {
        flex-direction: column;
        gap: 0.5rem;
    }

    .navbar-content {
        flex-direction: column;
        gap: 1rem;
    }

    .nav-menu {
        gap: 1rem;
    }

    .hero-content,
    .about-content,
    .contact-content {
        grid-template-columns: 1fr;
    }

    .hero-text h1 {
        font-size: 2.2rem;
    }

    .hero-buttons {
        flex-direction: column;
    }

    .about-images {
        order: 2;
    }

    .about-text {
        order: 1;
    }

    .services-grid,
    .process-grid {
        grid-template-columns: 1fr;
    }

    .free-consultation-btn {
        width: 100%;
    }
}

@media (max-width: 480px) {
    .hero-text h1 {
        font-size: 1.8rem;
    }

    .services-header h2,
    .about-text h2 {
        font-size: 1.8rem;
    }

    .nav-menu {
        display: none;
    }
}
