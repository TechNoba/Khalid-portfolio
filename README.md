<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Khalid Jibril | Web3 Professional</title>
    <meta name="description" content="Khalid Jibril, Web3 enthusiast, educator, and community builder from Africa. Specializing in AI-powered bots, Web3 content, and community management.">
    <meta name="keywords" content="Web3, blockchain, community management, AI bots, Khalid Jibril, SkillBridge, Crypto Basic Hub">
    <meta property="og:title" content="Khalid Jibril | Web3 Professional">
    <meta property="og:description" content="Empowering Web3 innovation with community building, AI solutions, and content creation.">
    <meta property="og:image" content="https://khalidjibril.com/profile.jpg">
    <meta property="og:url" content="https://khalidjibril.com">
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <script src="https://unpkg.com/scrollreveal@4.0.9/dist/scrollreveal.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap');
        
        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #10b981;
            --accent: #facc15;
            --dark: #0f172a;
            --light: #f8fafc;
        }
        
        body {
            font-family: 'Space Grotesk', sans-serif;
            background-color: var(--dark);
            color: var(--light);
            overflow-x: hidden;
            line-height: 1.7;
        }
        
        .gradient-text {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .card-hover {
            transition: all 0.3s ease;
            transform-style: preserve-3d;
        }
        
        .card-hover:hover {
            transform: translateY(-10px) rotateX(5deg);
            box-shadow: 0 25px 50px -12px rgba(99, 102, 241, 0.3);
        }
        
        .service-card {
            perspective: 1000px;
        }
        
        .floating {
            animation: floating 6s ease-in-out infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .contact-btn {
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px -1px rgba(99, 102, 241, 0.3), 0 2px 4px -1px rgba(99, 102, 241, 0.1);
        }
        
        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.3), 0 4px 6px -2px rgba(99, 102, 241, 0.1);
        }
        
        .glow {
            animation: glow 2s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from { box-shadow: 0 0 5px rgba(99, 102, 241, 0.5); }
            to { box-shadow: 0 0 20px rgba(99, 102, 241, 0.8); }
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            margin: 10px auto 0;
            border-radius: 2px;
        }
        
        .modal {
            transition: all 0.3s ease;
            transform: scale(0.9);
            opacity: 0;
            visibility: hidden;
        }
        
        .modal.active {
            transform: scale(1);
            opacity: 1;
            visibility: visible;
        }
        
        .bg-particle {
            position: absolute;
            width: 2px;
            height: 2px;
            background-color: rgba(99, 102, 241, 0.5);
            border-radius: 50%;
            pointer-events: none;
        }

        .text-gray-400 {
            color: #94a3b8;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 50%;
        }
    </style>
</head>
<body class="min-h-screen bg-dark">
    <!-- Particle Background -->
    <div id="particles"></div>
    
    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-dark/80 backdrop-blur-sm border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex items-center">
                    <span class="text-xl font-bold gradient-text">KhalidJibril</span>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-300 hover:text-accent transition">Home</a>
                    <a href="#about" class="text-gray-300 hover:text-accent transition">About</a>
                    <a href="#projects" class="text-gray-300 hover:text-accent transition">Projects</a>
                    <a href="#services" class="text-gray-300 hover:text-accent transition">Services</a>
                    <a href="#contact" class="bg-primary px-4 py-2 rounded-lg text-white hover:bg-primary-dark transition contact-btn">Contact</a>
                </div>
                <div class="md:hidden">
                    <button id="menu-toggle" class="text-gray-300 hover:text-accent focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-dark/95 backdrop-blur-sm pb-4 px-4">
            <div class="flex flex-col space-y-3">
                <a href="#home" class="text-gray-300 hover:text-accent transition py-2 border-b border-gray-800">Home</a>
                <a href="#about" class="text-gray-300 hover:text-accent transition py-2 border-b border-gray-800">About</a>
                <a href="#projects" class="text-gray-300 hover:text-accent transition py-2 border-b border-gray-800">Projects</a>
                <a href="#services" class="text-gray-300 hover:text-accent transition py-2 border-b border-gray-800">Services</a>
                <a href="#contact" class="bg-primary px-4 py-2 rounded-lg text-white hover:bg-primary-dark transition text-center mt-2 contact-btn">Contact</a>
            </div>
        </div>
    </nav>
    
    <!-- Hero Section -->
    <section id="home" class="pt-32 pb-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto relative overflow-hidden">
        <div class="absolute top-0 right-0 w-64 h-64 bg-primary rounded-full filter blur-3xl opacity-20 -z-10"></div>
        <div class="absolute bottom-0 left-0 w-64 h-64 bg-secondary rounded-full filter blur-3xl opacity-20 -z-10"></div>
        
        <div class="flex flex-col md:flex-row items-center justify-between">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold mb-6 leading-tight">
                    Hi, I'm <span class="gradient-text">Khalid Jibril</span>
                </h1>
                <div class="text-xl md:text-2xl mb-8 text-gray-300">
                    <span class="inline-block mr-4">Web3 Enthusiast</span>
                    <span class="inline-block mr-4">Educator</span>
                    <span class="inline-block mr-4">Community Builder</span>
                    <span class="inline-block">AI & Web Developer</span>
                </div>
                <p class="text-lg text-gray-400 mb-10 max-w-lg">
                    Empowering Web3 innovation across Africa through community building, AI solutions, and impactful content creation.
                </p>
                <div class="flex flex-wrap gap-4">
                    <button id="contact-trigger" class="bg-primary hover:bg-primary-dark text-white px-6 py-3 rounded-lg font-medium transition-all contact-btn glow">
                        Let's Work Together
                    </button>
                    <a href="https://t.me/SkillBridge_Hub" target="_blank" class="bg-secondary hover:bg-secondary/80 text-white px-6 py-3 rounded-lg font-medium transition-all contact-btn">
                        Join SkillBridge Hub
                    </a>
                    <a href="https://t.me/CryptoBasicHub_AF" target="_blank" class="border border-accent text-accent hover:bg-accent/10 px-6 py-3 rounded-lg font-medium transition-all">
                        Join Crypto Basic Hub
                    </a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div class="relative w-64 h-64 sm:w-80 sm:h-80">
                    <div class="absolute inset-0 bg-gradient-to-br from-primary to-secondary rounded-2xl opacity-20 blur-xl"></div>
                    <div class="relative bg-dark border border-gray-800 rounded-2xl p-1 w-full h-full overflow-hidden">
                        <div class="absolute inset-0 bg-gradient-to-br from-primary/10 to-secondary/10 opacity-30"></div>
                        <div class="absolute inset-0 flex items-center justify-center">
                            <div class="w-32 h-32 bg-primary rounded-full filter blur-2xl opacity-20"></div>
                        </div>
                        <div class="relative z-10 w-full h-full flex items-center justify-center">
                            <div class="text-center p-6">
                                <div class="w-24 h-24 sm:w-32 sm:h-32 mx-auto mb-6 rounded-full bg-gradient-to-br from-primary to-secondary flex items-center justify-center overflow-hidden">
                                    <img src="profile.jpg" alt="Profile picture of Khalid Jibril" class="profile-img" loading="lazy">
                                </div>
                                <h3 class="text-xl font-bold text-white mb-2">Web3 Builder</h3>
                                <p class="text-gray-400 text-sm">Connecting Africa to Blockchain</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="py-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto">
        <div class="text-center mb-16">
            <h2 class="text-3xl sm:text-4xl font-bold mb-4 section-title">About Me</h2>
            <p class="text-gray-400 max-w-3xl mx-auto">Web3 enthusiast and tech-driven problem solver from Africa</p>
        </div>
        
        <div class="flex flex-col md:flex-row gap-10 items-center">
            <div class="md:w-1/2">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 card-hover">
                    <p class="text-gray-300 mb-6">
                        I'm a Web3 enthusiast and tech-driven problem solver from Africa. I founded <a href="https://t.me/CryptoBasicHub_AF" target="_blank" class="text-primary font-medium hover:underline">Crypto Basic Hub</a>, a fast-growing educational community where I simplify blockchain, crypto, and decentralized tech for beginners.
                    </p>
                    <p class="text-gray-300 mb-6">
                        I'm also the founder of <a href="https://t.me/SkillBridge_Hub" target="_blank" class="text-secondary font-medium hover:underline">SkillBridge</a> — a curated network connecting Web3 talents from Africa and Asia with real opportunities. SkillBridge isn't just a community — it's a movement.
                    </p>
                    <p class="text-gray-300">
                        Over the years, I've taught myself development, community building, and content creation by doing — testing ideas, failing, and improving. Now I help projects find their voice, grow their user base, and build for long-term impact.
                    </p>
                </div>
            </div>
            <div class="md:w-1/2">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <h3 class="text-xl font-bold text-white mb-6">Partnerships & Roles</h3>
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-primary/10 p-3 rounded-lg mr-4">
                                <i class="fas fa-rocket text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-white mb-1">Africa Ambassador of Moonrig</h4>
                                <p class="text-gray-400 text-sm">Expanding Moonrig's presence across Africa</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-secondary/10 p-3 rounded-lg mr-4">
                                <i class="fas fa-handshake text-secondary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-white mb-1">Partner of TappRank</h4>
                                <p class="text-gray-400 text-sm">Collaborating on Web3 projects and community growth</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-purple-500/10 p-3 rounded-lg mr-4">
                                <i class="fas fa-coins text-purple-500"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-white mb-1">Partner of Farmaton</h4>
                                <p class="text-gray-400 text-sm">Working on airdrop campaigns and engagement</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-yellow-500/10 p-3 rounded-lg mr-4">
                                <i class="fas fa-parachute-box text-yellow-500"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-white mb-1">Amonia Airdrops Partner</h4>
                                <p class="text-gray-400 text-sm">Coordinating strategic airdrop campaigns</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Projects Section -->
    <section id="projects" class="py-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto bg-gray-900/30">
        <div class="text-center mb-16">
            <h2 class="text-3xl sm:text-4xl font-bold mb-4 section-title">My Projects</h2>
            <p class="text-gray-400 max-w-3xl mx-auto">Showcasing impactful Web3 initiatives and communities</p>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-primary/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-users text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Crypto Basic Hub</h3>
                    <p class="text-gray-400 mb-4">
                        Founded a Telegram community with 5,000+ members, educating Africans on blockchain and crypto basics.
                    </p>
                    <a href="https://t.me/CryptoBasicHub_AF" target="_blank" class="text-primary hover:underline">Join Now</a>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-secondary/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-bridge text-secondary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">SkillBridge Hub</h3>
                    <p class="text-gray-400 mb-4">
                        A network connecting Web3 talents from Africa and Asia to global opportunities.
                    </p>
                    <a href="https://t.me/SkillBridge_Hub" target="_blank" class="text-secondary hover:underline">Join Now</a>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-accent/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-rocket text-accent text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Moonrig Ambassadorship</h3>
                    <p class="text-gray-400 mb-4">
                        Leading Moonrig's expansion in Africa through community engagement and promotions.
                    </p>
                    <a href="https://moonrig.io" target="_blank" class="text-accent hover:underline">Learn More</a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Services Section -->
    <section id="services" class="py-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto bg-gray-900/30">
        <div class="text-center mb-16">
            <h2 class="text-3xl sm:text-4xl font-bold mb-4 section-title">What I Offer</h2>
            <p class="text-gray-400 max-w-3xl mx-auto">Comprehensive Web3 solutions tailored to your project's needs</p>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-primary/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-robot text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">AI-Powered Support Bots</h3>
                    <p class="text-gray-400 mb-4">
                        Custom AI chatbots for 24/7 support, user onboarding, and automation for Web3 projects.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-primary/10 text-primary text-xs px-3 py-1 rounded-full">ChatGPT</span>
                        <span class="bg-primary/10 text-primary text-xs px-3 py-1 rounded-full">Automation</span>
                        <span class="bg-primary/10 text-primary text-xs px-3 py-1 rounded-full">24/7 Support</span>
                    </div>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-secondary/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-pen-fancy text-secondary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Content Creation</h3>
                    <p class="text-gray-400 mb-4">
                        Engaging Web3 tutorials, explainers, and marketing content to educate and attract audiences.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-secondary/10 text-secondary text-xs px-3 py-1 rounded-full">Web3 Education</span>
                        <span class="bg-secondary/10 text-secondary text-xs px-3 py-1 rounded-full">Tutorials</span>
                        <span class="bg-secondary/10 text-secondary text-xs px-3 py-1 rounded-full">Marketing</span>
                    </div>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-purple-500/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-users text-purple-500 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Community Management</h3>
                    <p class="text-gray-400 mb-4">
                        Building and managing vibrant Web3 communities with a focus on engagement and growth.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-purple-500/10 text-purple-500 text-xs px-3 py-1 rounded-full">Engagement</span>
                        <span class="bg-purple-500/10 text-purple-500 text-xs px-3 py-1 rounded-full">Growth</span>
                        <span class="bg-purple-500/10 text-purple-500 text-xs px-3 py-1 rounded-full">Moderation</span>
                    </div>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-yellow-500/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-bullhorn text-yellow-500 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Promotions & Campaigns</h3>
                    <p class="text-gray-400 mb-4">
                        Strategic airdrops, AMAs, and KOL campaigns to reach 10k–200k+ users.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-yellow-500/10 text-yellow-500 text-xs px-3 py-1 rounded-full">Airdrops</span>
                        <span class="bg-yellow-500/10 text-yellow-500 text-xs px-3 py-1 rounded-full">AMAs</span>
                        <span class="bg-yellow-500/10 text-yellow-500 text-xs px-3 py-1 rounded-full">KOLs</span>
                    </div>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-blue-500/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-code text-blue-500 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Website Development</h3>
                    <p class="text-gray-400 mb-4">
                        Professional, responsive websites optimized for Web3 projects and startups.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-blue-500/10 text-blue-500 text-xs px-3 py-1 rounded-full">Web Design</span>
                        <span class="bg-blue-500/10 text-blue-500 text-xs px-3 py-1 rounded-full">Responsive</span>
                        <span class="bg-blue-500/10 text-blue-500 text-xs px-3 py-1 rounded-full">SEO</span>
                    </div>
                </div>
            </div>
            <div class="service-card">
                <div class="bg-gray-900/50 border border-gray-800 rounded-2xl p-8 h-full card-hover">
                    <div class="bg-pink-500/10 w-14 h-14 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-paper-plane text-pink-500 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">Airdrop Automation</h3>
                    <p class="text-gray-400 mb-4">
                        Scalable airdrop bots with referral systems and leaderboards for viral growth.
                    </p>
                    <div class="flex flex-wrap gap-2 mt-6">
                        <span class="bg-pink-500/10 text-pink-500 text-xs px-3 py-1 rounded-full">Automation</span>
                        <span class="bg-pink-500/10 text-pink-500 text-xs px-3 py-1 rounded-full">Referrals</span>
                        <span class="bg-pink-500/10 text-pink-500 text-xs px-3 py-1 rounded-full">Leaderboards</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- CTA Section -->
    <section class="py-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto relative overflow-hidden">
        <div class="absolute inset-0 bg-gradient-to-r from-primary/10 to-secondary/10 rounded-3xl -z-10"></div>
        <div class="text-center">
            <h2 class="text-3xl sm:text-4xl font-bold mb-6">Let's Build Something <span class="gradient-text">Meaningful</span> Together</h2>
            <p class="text-xl text-gray-300 max-w-3xl mx-auto mb-10">
                Ready to grow your Web3 project? I offer community management, AI solutions, and strategic promotions tailored to your vision.
            </p>
            <button id="contact-trigger-2" class="bg-primary hover:bg-primary-dark text-white px-8 py-4 rounded-lg font-medium text-lg transition-all contact-btn glow">
                Get In Touch
            </button>
        </div>
    </section>
    
    <!-- Contact Modal -->
    <div id="contact-modal" class="fixed inset-0 bg-black/80 z-50 flex items-center justify-center p-4 modal">
        <div class="bg-gray-900 border border-gray-800 rounded-2xl max-w-md w-full p-8 relative">
            <button id="close-modal" class="absolute top-4 right-4 text-gray-400 hover:text-white">
                <i class="fas fa-times text-xl"></i>
            </button>
            <h3 class="text-2xl font-bold text-white mb-6 text-center">Contact Me</h3>
            <form action="https://getform.io/f/ajjojzja" method="POST" class="space-y-4">
                <div>
                    <label for="name" class="block text-sm font-medium text-gray-300">Name</label>
                    <input type="text" id="name" name="name" class="w-full mt-1 p-3 bg-gray-800 border border-gray-700 rounded-lg text-white focus:ring-primary focus:border-primary" required>
                </div>
                <div>
                    <label for="email" class="block text-sm font-medium text-gray-300">Email</label>
                    <input type="email" id="email" name="email" class="w-full mt-1 p-3 bg-gray-800 border border-gray-700 rounded-lg text-white focus:ring-primary focus:border-primary" required>
                </div>
                <div>
                    <label for="message" class="block text-sm font-medium text-gray-300">Message</label>
                    <textarea id="message" name="message" rows="4" class="w-full mt-1 p-3 bg-gray-800 border border-gray-700 rounded-lg text-white focus:ring-primary focus:border-primary" required></textarea>
                </div>
                <button type="submit" class="w-full bg-primary hover:bg-primary-dark text-white px-6 py-3 rounded-lg font-medium transition-all contact-btn">Send Message</button>
            </form>
            <div class="mt-6 pt-6 border-t border-gray-800">
                <h4 class="text-sm font-medium text-gray-400 mb-3">Or connect directly:</h4>
                <div class="space-y-4">
                    <a href="https://twitter.com/AI_Mentee" target="_blank" class="flex items-center justify-center bg-gray-800 hover:bg-gray-700 text-white px-6 py-3 rounded-lg transition">
                        <i class="fab fa-twitter mr-3 text-blue-400"></i>
                        Message on X (Twitter)
                    </a>
                    <a href="https://t.me/AI_Mentee" target="_blank" class="flex items-center justify-center bg-gray-800 hover:bg-gray-700 text-white px-6 py-3 rounded-lg transition">
                        <i class="fab fa-telegram-plane mr-3 text-blue-500"></i>
                        Message on Telegram
                    </a>
                    <a href="https://discord.com/users/ai_mentee" class="flex items-center justify-center bg-gray-800 hover:bg-gray-700 text-white px-6 py-3 rounded-lg transition">
                        <i class="fab fa-discord mr-3 text-blue-500"></i>
                        Message on Discord
                    </a>
                    <a href="mailto:khaleedjibreel64@gmail.com" class="flex items-center justify-center bg-gray-800 hover:bg-gray-700 text-white px-6 py-3 rounded-lg transition">
                        <i class="fas fa-envelope mr-3 text-secondary"></i>
                        Send an Email
                    </a>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Footer -->
    <footer class="py-12 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto border-t border-gray-800">
        <div class="flex flex-col md:flex-row justify-between items-center">
            <div class="mb-6 md:mb-0">
                <span class="text-xl font-bold gradient-text">Khalid Jibril</span>
                <p class="text-gray-400 mt-2">Web3 Enthusiast | Educator | Community Builder</p>
            </div>
            <div class="flex flex-col md:flex-row gap-6 items-center">
                <div class="flex space-x-6">
                    <a href="https://twitter.com/AI_Mentee" class="text-gray-400 hover:text-accent transition">
                        <i class="fab fa-twitter text-xl"></i>
                    </a>
                    <a href="https://t.me/AI_Mentee" class="text-gray-400 hover:text-accent transition">
                        <i class="fab fa-telegram-plane text-xl"></i>
                    </a>
                    <a href="https://discord.com/users/ai_mentee" class="text-gray-400 hover:text-accent transition">
                        <i class="fab fa-discord text-xl"></i>
                    </a>
                </div>
                <div class="flex gap-4 mt-4 md:mt-0">
                    <a href="https://t.me/SkillBridge_Hub" target="_blank" class="bg-secondary hover:bg-secondary/80 text-white px-4 py-2 rounded-lg font-medium transition-all">
                        SkillBridge Hub
                    </a>
                    <a href="https://t.me/CryptoBasicHub_AF" target="_blank" class="bg-primary hover:bg-primary-dark text-white px-4 py-2 rounded-lg font-medium transition-all">
                        Crypto Basic Hub
                    </a>
                </div>
            </div>
        </div>
        <div class="mt-8 text-center text-gray-500 text-sm">
            <p>© 2025 Khalid Jibril. All rights reserved.</p>
        </div>
    </footer>
    
    <script>
        // Mobile menu toggle
        const menuToggle = document.getElementById('menu-toggle');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuToggle.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Contact modal
        const contactTriggers = document.querySelectorAll('[id^="contact-trigger"]');
        const contactModal = document.getElementById('contact-modal');
        const closeModal = document.getElementById('close-modal');
        
        contactTriggers.forEach(trigger => {
            trigger.addEventListener('click', () => {
                contactModal.classList.add('active');
                document.body.style.overflow = 'hidden';
            });
        });
        
        closeModal.addEventListener('click', () => {
            contactModal.classList.remove('active');
            document.body.style.overflow = '';
        });
        
        contactModal.addEventListener('click', (e) => {
            if (e.target === contactModal) {
                contactModal.classList.remove('active');
                document.body.style.overflow = '';
            }
        });
        
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Scroll reveal
        const sr = ScrollReveal({
            origin: 'bottom',
            distance: '60px',
            duration: 1000,
            delay: 200,
            reset: false
        });
        
        sr.reveal('#home > div', { origin: 'left' });
        sr.reveal('.section-title', { origin: 'top' });
        sr.reveal('#about > div > div', { interval: 200 });
        sr.reveal('#projects .service-card', { interval: 200 });
        sr.reveal('#services .service-card', { interval: 200 });
        
        // Optimized particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 30;
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('bg-particle');
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                const size = Math.random() * 2 + 1;
                const opacity = Math.random() * 0.4 + 0.1;
                const duration = Math.random() * 15 + 8;
                const delay = Math.random() * 4;
                particle.style.left = `${posX}%`;
                particle.style.top = `${posY}%`;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.opacity = opacity;
                particle.style.animation = `floating ${duration}s ease-in-out ${delay}s infinite`;
                particlesContainer.appendChild(particle);
            }
        }
        
        document.addEventListener('DOMContentLoaded', createParticles);
        
        // Parallax effect
        document.addEventListener('mousemove', (e) => {
            const cards = document.querySelectorAll('.card-hover');
            cards.forEach(card => {
                const rect = card.getBoundingClientRect();
                const x = e.clientX - rect.left;
                const y = e.clientY - rect.top;
                const centerX = rect.width / 2;
                const centerY = rect.height / 2;
                const angleX = (y - centerY) / 20;
                const angleY = (centerX - x) / 20;
                card.style.transform = `perspective(1000px) rotateX(${angleX}deg) rotateY(${angleY}deg)`;
            });
        });
        
        document.querySelectorAll('.card-hover').forEach(card => {
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'perspective(1000px) rotateX(0) rotateY(0)';
            });
        });
    </script>
</body>
</html>