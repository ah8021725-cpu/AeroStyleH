<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hero Style H - Timeless Elegance • Heroic Legacy</title>
    <meta name="description" content="Hero Style H - Ultra-luxury lifestyle brand featuring premium jewelry, watches, jackets, shoes and innerwear. Timeless elegance meets heroic legacy.">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;500;600;700;800&family=Playfair+Display:wght@400;500;600;700;800;900&display=swap');
        
        body {
            font-family: 'Playfair Display', serif;
            background: linear-gradient(135deg, #0A0A0A 0%, #1A1A1A 50%, #0A0A0A 100%);
            overflow-x: hidden;
        }
        .hero-gradient {
            background: radial-gradient(ellipse at center, rgba(212, 175, 119, 0.1) 0%, transparent 70%);
        }
        .gold-glow {
            box-shadow: 0 0 30px rgba(212, 175, 119, 0.4);
        }
        .glassmorphism {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(212, 175, 119, 0.2);
        }
        .product-hover {
            transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .product-hover:hover {
            transform: translateY(-15px) scale(1.02);
            box-shadow: 0 30px 60px rgba(212, 175, 119, 0.3);
        }
        .gold-shine {
            background: linear-gradient(45deg, #D4AF77, #F2D492, #D4AF77);
            background-size: 300% 300%;
            animation: shine 2s infinite;
        }
        @keyframes shine {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .sparkle {
            position: relative;
        }
        .sparkle::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, transparent, rgba(212, 175, 119, 0.3), transparent);
            border-radius: inherit;
            z-index: -1;
            opacity: 0;
            transition: opacity 0.3s;
        }
        .sparkle:hover::before {
            opacity: 1;
            animation: sparkle 1.5s infinite;
        }
        @keyframes sparkle {
            0%, 100% { transform: scale(1) rotate(0deg); }
            50% { transform: scale(1.1) rotate(180deg); }
        }
        .section-title {
            font-family: 'Cinzel', serif;
            background: linear-gradient(135deg, #D4AF77, #F2D492);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .mobile-menu {
            transform: translateX(100%);
            transition: transform 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .mobile-menu.open {
            transform: translateX(0);
        }
    </style>
</head>
<body class="text-white min-h-screen">
    <!-- Loading Screen -->
    <div id="loader" class="fixed inset-0 bg-black z-50 flex items-center justify-center">
        <div class="w-24 h-24 border-4 border-gold-shine/30 border-t-gold-shine rounded-full animate-spin"></div>
    </div>

    <!-- Sticky Navigation -->
    <nav id="navbar" class="fixed top-0 left-0 right-0 z-40 glassmorphism transition-all duration-500">
        <div class="max-w-7xl mx-auto px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <h1 class="text-3xl lg:text-4xl font-black section-title sparkle cursor-pointer" onclick="scrollToSection('home')">Hero Style H</h1>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('home')">
                        Home
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#jewelry" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('jewelry')">
                        Jewelry
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#watches" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('watches')">
                        Watches
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#jackets" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('jackets')">
                        Jackets
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#shoes" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('shoes')">
                        Shoes
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#underwear" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('underwear')">
                        Innerwear
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                    <a href="#heritage" class="nav-link text-lg font-medium hover:text-gold-glow transition-all duration-300 relative group" onclick="scrollToSection('heritage')">
                        Heritage
                        <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-gold-shine to-transparent group-hover:w-full transition-all duration-300"></span>
                    </a>
                </div>

                <!-- Right Icons -->
                <div class="flex items-center space-x-4">
                    <button class="p-2 hover:bg-white/10 rounded-full transition-all duration-300" onclick="toggleSearch()">
                        <i class="fas fa-search text-xl"></i>
                    </button>
                    <button class="p-2 hover:bg-white/10 rounded-full transition-all duration-300 relative">
                        <i class="fas fa-heart text-xl"></i>
                        <span class="absolute -top-1 -right-1 w-5 h-5 bg-red-500 text-xs rounded-full flex items-center justify-center">3</span>
                    </button>
                    <button id="cartBtn" class="p-2 hover:bg-white/10 rounded-full transition-all duration-300 relative" onclick="openCart()">
                        <i class="fas fa-shopping-bag text-xl"></i>
                        <span class="absolute -top-1 -right-1 w-5 h-5 bg-gold-shine text-black text-xs rounded-full flex items-center justify-center font-bold">2</span>
                    </button>
                    <button id="mobileMenuBtn" class="p-2 hover:bg-white/10 rounded-full transition-all duration-300 md:hidden" onclick="toggleMobileMenu()">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobileMenu" class="mobile-menu md:hidden fixed top-20 right-0 w-64 h-screen glassmorphism z-50 p-8">
            <button onclick="toggleMobileMenu()" class="absolute top-6 right-6 text-2xl">&times;</button>
            <div class="flex flex-col space-y-6 mt-12">
                <a href="#home" class="text-xl font-semibold py-2" onclick="scrollToSection('home'); toggleMobileMenu()">Home</a>
                <a href="#jewelry" class="text-xl font-semibold py-2" onclick="scrollToSection('jewelry'); toggleMobileMenu()">Jewelry</a>
                <a href="#watches" class="text-xl font-semibold py-2" onclick="scrollToSection('watches'); toggleMobileMenu()">Watches</a>
                <a href="#jackets" class="text-xl font-semibold py-2" onclick="scrollToSection('jackets'); toggleMobileMenu()">Jackets</a>
                <a href="#shoes" class="text-xl font-semibold py-2" onclick="scrollToSection('shoes'); toggleMobileMenu()">Shoes</a>
                <a href="#underwear" class="text-xl font-semibold py-2" onclick="scrollToSection('underwear'); toggleMobileMenu()">Innerwear</a>
                <a href="#heritage" class="text-xl font-semibold py-2" onclick="scrollToSection('heritage'); toggleMobileMenu()">Heritage</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center relative overflow-hidden hero-gradient pt-20">
        <canvas id="particles-js" class="absolute inset-0 z-10"></canvas>
        
        <div class="text-center z-20 px-6 max-w-4xl mx-auto">
            <h1 class="text-6xl lg:text-8xl font-black section-title mb-8 leading-tight">
                Hero Style H
            </h1>
            <p class="text-2xl lg:text-3xl font-light mb-12 opacity-90 max-w-2xl mx-auto leading-relaxed">
                Timeless Elegance • Heroic Legacy
            </p>
            <div class="flex flex-col sm:flex-row gap-6 justify-center items-center">
                <a href="#featured" class="gold-shine text-black font-semibold py-4 px-12 rounded-full text-lg shadow-2xl gold-glow hover:scale-105 transition-all duration-300 sparkle" onclick="scrollToSection('featured')">
                    Shop Now
                </a>
                <a href="#jewelry" class="border-2 border-gold-shine text-gold-shine font-semibold py-4 px-12 rounded-full text-lg hover:bg-gold-shine hover:text-black transition-all duration-300 sparkle" onclick="scrollToSection('jewelry')">
                    Explore Collections
                </a>
            </div>
        </div>
        
        <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 animate-bounce">
            <i class="fas fa-chevron-down text-2xl text-gold-shine cursor-pointer hover:scale-110 transition-all duration-300" onclick="scrollToSection('featured')"></i>
        </div>
    </section>

    <!-- Featured Collections -->
    <section id="featured" class="py-32 px-6 max-w-7xl mx-auto">
        <div class="text-center mb-24">
            <h2 class="section-title text-5xl lg:text-7xl font-black mb-6">Featured Collections</h2>
            <p class="text-xl lg:text-2xl opacity-80 max-w-3xl mx-auto">Discover our signature collections crafted for the modern gentleman</p>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-8">
            <a href="#jewelry" class="group relative overflow-hidden rounded-3xl glassmorphism p-8 text-center hover:bg-white/10 transition-all duration-500 cursor-pointer" onclick="scrollToSection('jewelry')">
                <div class="w-24 h-24 bg-gradient-to-br from-gold-shine to-transparent rounded-2xl mx-auto mb-6 group-hover:scale-110 transition-transform duration-300"></div>
                <h3 class="text-2xl font-bold mb-2 group-hover:text-gold-shine transition-all duration-300">Jewelry</h3>
                <p class="opacity-70">18K Gold • Diamonds</p>
            </a>
            <a href="#watches" class="group relative overflow-hidden rounded-3xl glassmorphism p-8 text-center hover:bg-white/10 transition-all duration-500 cursor-pointer" onclick="scrollToSection('watches')">
                <div class="w-24 h-24 bg-gradient-to-br from-gold-shine to-transparent rounded-2xl mx-auto mb-6 group-hover:scale-110 transition-transform duration-300"></div>
                <h3 class="text-2xl font-bold mb-2 group-hover:text-gold-shine transition-all duration-300">Watches</h3>
                <p class="opacity-70">Swiss Precision</p>
            </a>
            <a href="#jackets" class="group relative overflow-hidden rounded-3xl glassmorphism p-8 text-center hover:bg-white/10 transition-all duration-500 cursor-pointer" onclick="scrollToSection('jackets')">
                <div class="w-24 h-24 bg-gradient-to-br from-gold-shine to-transparent rounded-2xl mx-auto mb-6 group-hover:scale-110 transition-transform duration-300"></div>
                <h3 class="text-2xl font-bold mb-2 group-hover:text-gold-shine transition-all duration-300">Jackets</h3>
                <p class="opacity-70">Italian Leather</p>
            </a>
            <a href="#shoes" class="group relative overflow-hidden rounded-3xl glassmorphism p-8 text-center hover:bg-white/10 transition-all duration-500 cursor-pointer" onclick="scrollToSection('shoes')">
                <div class="w-24 h-24 bg-gradient-to-br from-gold-shine to-transparent rounded-2xl mx-auto mb-6 group-hover:scale-110 transition-transform duration-300"></div>
                <h3 class="text-2xl font-bold mb-2 group-hover:text-gold-shine transition-all duration-300">Shoes</h3>
                <p class="opacity-70">Handcrafted</p>
            </a>
            <a href="#underwear" class="group relative overflow-hidden rounded-3xl glassmorphism p-8 text-center hover:bg-white/10 transition-all duration-500
