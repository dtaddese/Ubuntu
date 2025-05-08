<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ubuntu Construction Solutions | Sustainable Building Materials</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'ubuntu-darker': '#434a49',
                        'ubuntu-dark': '#596364',
                        'ubuntu-green': '#388E3C',
                        'ubuntu-light-green': '#7CB342',
                        'ubuntu-lighter-green': '#C0CA33',
                    }
                }
            }
        }
    </script>
    <style>
        .hero-section {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
        }
        
        .impact-card {
            transition: all 0.3s ease;
        }
        
        .impact-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .material-card {
            transition: all 0.3s ease;
        }
        
        .material-card:hover {
            transform: scale(1.05);
        }
        
        .testimonial-slide {
            display: none;
        }
        
        .testimonial-slide.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #7CB342;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
    </style>
</head>
<body class="font-sans">
    <!-- Navigation -->
    <nav class="bg-ubuntu-darker text-white sticky top-0 z-50 shadow-lg">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <div class="w-12 h-12 rounded-full bg-ubuntu-green flex items-center justify-center mr-3">
                    <i class="fas fa-leaf text-white text-xl"></i>
                </div>
                <span class="text-2xl font-bold">Ubuntu<span class="text-ubuntu-light-green">Construction</span></span>
            </div>
            
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link">Home</a>
                <a href="#solutions" class="nav-link">Solutions</a>
                <a href="#materials" class="nav-link">Materials</a>
                <a href="#impact" class="nav-link">Impact</a>
                <a href="#services" class="nav-link">Services</a>
                <a href="#contact" class="nav-link">Contact</a>
            </div>
            
            <button class="md:hidden text-white focus:outline-none" id="mobile-menu-button">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- Mobile Menu -->
        <div class="md:hidden hidden bg-ubuntu-dark w-full py-2 px-4" id="mobile-menu">
            <div class="flex flex-col space-y-3">
                <a href="#home" class="nav-link py-2">Home</a>
                <a href="#solutions" class="nav-link py-2">Solutions</a>
                <a href="#materials" class="nav-link py-2">Materials</a>
                <a href="#impact" class="nav-link py-2">Impact</a>
                <a href="#services" class="nav-link py-2">Services</a>
                <a href="#contact" class="nav-link py-2">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section text-white py-20 md:py-32">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">Building a <span class="text-ubuntu-light-green">Sustainable</span> Future</h1>
            <p class="text-xl md:text-2xl mb-8 max-w-3xl mx-auto">Affordable, eco-friendly construction materials and land restoration solutions that create jobs while healing the planet.</p>
            <div class="flex flex-col md:flex-row justify-center gap-4">
                <a href="#contact" class="bg-ubuntu-green hover:bg-ubuntu-light-green text-white font-bold py-3 px-8 rounded-full transition duration-300">Get Started</a>
                <a href="#solutions" class="border-2 border-white hover:bg-white hover:text-ubuntu-darker text-white font-bold py-3 px-8 rounded-full transition duration-300">Learn More</a>
            </div>
        </div>
    </section>

    <!-- Sustainable Solutions -->
    <section id="solutions" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">Our <span class="text-ubuntu-green">Sustainable</span> Solutions</h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">Innovative approaches to construction that helps make the dream of home ownership affordable and reclaim abandoned mines for Agricultural use</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300 border-t-4 border-ubuntu-green">
                    <div class="w-16 h-16 bg-ubuntu-light-green rounded-full flex items-center justify-center mb-4 mx-auto">
                        <i class="fas fa-recycle text-white text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-3 text-ubuntu-darker">Eco-Friendly Materials</h3>
                    <p class="text-gray-600 text-center">Sand, laterite-mortar-cement bricks, terrazzo, and granitic tiles produced using our patented zero-waste process.</p>
                </div>
                
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300 border-t-4 border-ubuntu-light-green">
                    <div class="w-16 h-16 bg-ubuntu-green rounded-full flex items-center justify-center mb-4 mx-auto">
                        <i class="fas fa-tree text-white text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-3 text-ubuntu-darker">Wood-Plastic Composites</h3>
                    <p class="text-gray-600 text-center">Trunks of Lantana camara and bamboo are repurposed into wood-plastic composites for partitioning, flooring, and ceilings.</p>
                </div>
                
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300 border-t-4 border-ubuntu-lighter-green">
                    <div class="w-16 h-16 bg-ubuntu-light-green rounded-full flex items-center justify-center mb-4 mx-auto">
                        <i class="fas fa-tractor text-white text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-3 text-ubuntu-darker">Land Restoration</h3>
                    <p class="text-gray-600 text-center">Rehabilitating abandoned mining sites into productive farmland using climate-resilient plants and sustainable techniques.</p>
                </div>
                
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition duration-300 border-t-4 border-ubuntu-green">
                    <div class="w-16 h-16 bg-ubuntu-lighter-green rounded-full flex items-center justify-center mb-4 mx-auto">
                        <i class="fas fa-users text-white text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-3 text-ubuntu-darker">Job Creation</h3>
                    <p class="text-gray-600 text-center">Transitioning illegal miners into formal, safe employment with fair wages and career development opportunities.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Construction Materials -->
    <section id="materials" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">Our <span class="text-ubuntu-green">Construction</span> Materials</h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">High-quality, sustainable alternatives at half the market price to traditional building materials that are imported</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="material-card bg-gray-50 rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1605100804763-247f67b3557e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');"></div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Eco Sand</h3>
                        <p class="text-gray-600 mb-4">Responsibly sourced sand with minimal environmental impact, processed through our zero-waste system.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-ubuntu-green font-bold">From $12/m³</span>
                            <button class="text-ubuntu-light-green hover:text-ubuntu-green font-semibold">Learn More →</button>
                        </div>
                    </div>
                </div>
                
                <div class="material-card bg-gray-50 rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1616486338812-3dadae4b4ace?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80');"></div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Terrazzo Tiles</h3>
                        <p class="text-gray-600 mb-4">Beautiful, durable tiles made from recycled materials with a unique, sustainable manufacturing process.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-ubuntu-green font-bold">From $25/m²</span>
                            <button class="text-ubuntu-light-green hover:text-ubuntu-green font-semibold">Learn More →</button>
                        </div>
                    </div>
                </div>
                
                <div class="material-card bg-gray-50 rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1600585152220-90363fe7e115?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');"></div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Granitic Tiles</h3>
                        <p class="text-gray-600 mb-4">Premium tiles crafted from locally sourced granite with minimal processing for maximum sustainability.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-ubuntu-green font-bold">From $30/m²</span>
                            <button class="text-ubuntu-light-green hover:text-ubuntu-green font-semibold">Learn More →</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Impact Section -->
    <section id="impact" class="py-16 bg-ubuntu-green text-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Our Measurable <span class="text-ubuntu-lighter-green">Impact</span></h2>
                <p class="text-lg max-w-3xl mx-auto">Quantifiable results that demonstrate our commitment to sustainability and community</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="impact-card bg-white text-ubuntu-darker p-8 rounded-lg text-center shadow-lg">
                    <div class="text-6xl font-bold text-ubuntu-green mb-4">100+</div>
                    <h3 class="text-xl font-bold mb-2">Acres of land restored</h3>
                    <p class="text-gray-600">Transforming abandoned mining sites into productive farmland</p>
                </div>
                
                <div class="impact-card bg-white text-ubuntu-darker p-8 rounded-lg text-center shadow-lg">
                    <div class="text-6xl font-bold text-ubuntu-light-green mb-4">1000+</div>
                    <h3 class="text-xl font-bold mb-2">Jobs created</h3>
                    <p class="text-gray-600">Providing formal employment with fair wages</p>
                </div>
                
                <div class="impact-card bg-white text-ubuntu-darker p-8 rounded-lg text-center shadow-lg">
                    <div class="text-6xl font-bold text-ubuntu-lighter-green mb-4">10,000+</div>
                    <h3 class="text-xl font-bold mb-2">Tons of CO₂ offset</h3>
                    <p class="text-gray-600">Through our sustainable materials and land restoration</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Land Restoration Process -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">From <span class="text-ubuntu-green">Mining Site</span> to <span class="text-ubuntu-light-green">Farmland</span></h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">Our land restoration program transforms abandoned mining sites into productive agricultural land</p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div>
                    <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Land restoration" class="rounded-lg shadow-lg w-full">
                </div>
                
                <div>
                    <p class="text-gray-600 mb-6">Silt-clay particles recovered during processing are used to backfill abandoned mines, making terraces to prevent the erosion and thus, improving soil texture and enabling afforestation efforts. Organic fertilizers and Lantana camara and bamboo are planted to enhance soil fertility, attract biodiversity, and accelerate land recovery.</p>
                    
                    <ul class="space-y-3">
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                            <span class="text-gray-700">Soil testing and remediation</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                            <span class="text-gray-700">Water management systems</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                            <span class="text-gray-700">Training for local farmers</span>
                        </li>
                    </ul>
                    
                    <button class="mt-6 bg-ubuntu-green hover:bg-ubuntu-light-green text-white font-bold py-2 px-6 rounded-full transition duration-300">Learn About Our Process</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">Our <span class="text-ubuntu-green">Services</span></h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">Multiple services that support our sustainability mission</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="bg-gray-50 p-6 rounded-lg border-l-4 border-ubuntu-green shadow-sm hover:shadow-md transition duration-300">
                    <div class="w-12 h-12 bg-ubuntu-green rounded-full flex items-center justify-center mb-4">
                        <i class="fas fa-store text-white"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Direct Sales</h3>
                    <p class="text-gray-600">Sand, laterite-mortar-cement bricks, terrazzo, and tiles sold directly to construction companies and developers.</p>
                </div>
                
                <div class="bg-gray-50 p-6 rounded-lg border-l-4 border-ubuntu-light-green shadow-sm hover:shadow-md transition duration-300">
                    <div class="w-12 h-12 bg-ubuntu-light-green rounded-full flex items-center justify-center mb-4">
                        <i class="fas fa-file-signature text-white"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Licensing</h3>
                    <p class="text-gray-600">Our proprietary zero-waste process and quarry management technology available for license.</p>
                </div>
                
                <div class="bg-gray-50 p-6 rounded-lg border-l-4 border-ubuntu-lighter-green shadow-sm hover:shadow-md transition duration-300">
                    <div class="w-12 h-12 bg-ubuntu-lighter-green rounded-full flex items-center justify-center mb-4">
                        <i class="fas fa-chalkboard-teacher text-white"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Consulting</h3>
                    <p class="text-gray-600">Expert services in exploration, land rehabilitation, and ESG compliance for mining and construction firms.</p>
                </div>
                
                <div class="bg-gray-50 p-6 rounded-lg border-l-4 border-ubuntu-green shadow-sm hover:shadow-md transition duration-300">
                    <div class="w-12 h-12 bg-ubuntu-green rounded-full flex items-center justify-center mb-4">
                        <i class="fas fa-coins text-white"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-ubuntu-darker">Carbon Credits</h3>
                    <p class="text-gray-600">Future revenue from monetizing carbon credits generated by our land restoration projects.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Investment Section -->
    <section class="py-16 bg-gradient-to-r from-ubuntu-darker to-ubuntu-dark text-white">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-6">Invest in <span class="text-ubuntu-light-green">Sustainability</span></h2>
                <p class="text-xl mb-8">We're seeking mission-aligned investors to help scale our impact. Join us in building a more sustainable construction industry.</p>
                
                <div class="grid md:grid-cols-2 gap-8 mb-10 text-left">
                    <div>
                        <h3 class="text-xl font-bold mb-4 text-ubuntu-lighter-green">Our Competitive Advantage</h3>
                        <ul class="space-y-3">
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Patented zero-waste technology</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Lower production costs through waste reduction</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Strong ESG credentials appealing to modern developers</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Government and NGO partnerships for land rehabilitation</span>
                            </li>
                        </ul>
                    </div>
                    
                    <div class="bg-white bg-opacity-10 p-6 rounded-lg">
                        <h3 class="text-xl font-bold mb-4 text-ubuntu-lighter-green">Investment Highlights</h3>
                        <ul class="space-y-3">
                            <li class="flex items-start">
                                <i class="fas fa-chart-line text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Projected 3-year ROI: 25-35%</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-globe-africa text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Scalable across multiple African markets</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-hand-holding-heart text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Positive social and environmental impact</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-shield-alt text-ubuntu-light-green mt-1 mr-2"></i>
                                <span>Diversified revenue streams</span>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <button class="bg-ubuntu-light-green hover:bg-ubuntu-lighter-green text-ubuntu-darker font-bold py-3 px-8 rounded-full transition duration-300">Request Investment Package</button>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">What Our <span class="text-ubuntu-green">Partners</span> Say</h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">Hear from those who have worked with us</p>
            </div>
            
            <div class="max-w-4xl mx-auto relative">
                <div class="testimonial-slide active bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-16 h-16 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Testimonial" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold text-lg">Sarah Johnson</h4>
                            <p class="text-ubuntu-light-green">Construction Manager, GreenBuild Co.</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Ubuntu's eco-friendly materials have allowed us to meet our sustainability targets while keeping costs competitive. Their terrazzo tiles are now our go-to choice for all our projects."</p>
                    <div class="flex mt-4">
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                    </div>
                </div>
                
                <div class="testimonial-slide bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-16 h-16 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Testimonial" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold text-lg">Michael Ofori</h4>
                            <p class="text-ubuntu-light-green">Director, Sustainable Mining Initiative</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"The land restoration work Ubuntu has done in our community is remarkable. They've transformed dangerous mining pits into productive farmland and created jobs for former illegal miners."</p>
                    <div class="flex mt-4">
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star-half-alt text-yellow-400"></i>
                    </div>
                </div>
                
                <div class="testimonial-slide bg-white p-8 rounded-lg shadow-md">
                    <div class="flex items-center mb-6">
                        <div class="w-16 h-16 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Testimonial" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold text-lg">Amina Diallo</h4>
                            <p class="text-ubuntu-light-green">CEO, EcoHomes Africa</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"As a developer focused on affordable, sustainable housing, Ubuntu's materials have been a game-changer. Their prices are competitive, and the quality exceeds expectations."</p>
                    <div class="flex mt-4">
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                        <i class="fas fa-star text-yellow-400"></i>
                    </div>
                </div>
                
                <div class="flex justify-center mt-8 space-x-2">
                    <button class="testimonial-dot w-3 h-3 rounded-full bg-ubuntu-green opacity-100" data-slide="0"></button>
                    <button class="testimonial-dot w-3 h-3 rounded-full bg-gray-300 opacity-50" data-slide="1"></button>
                    <button class="testimonial-dot w-3 h-3 rounded-full bg-gray-300 opacity-50" data-slide="2"></button>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-ubuntu-darker mb-4">Get In <span class="text-ubuntu-green">Touch</span></h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">Ready to build sustainably? Contact us for product information, consulting services, or partnership opportunities.</p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <form class="space-y-6">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Full Name</label>
                            <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-ubuntu-green focus:border-ubuntu-green">
                        </div>
                        
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email Address</label>
                            <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-ubuntu-green focus:border-ubuntu-green">
                        </div>
                        
                        <div>
                            <label for="phone" class="block text-sm font-medium text-gray-700 mb-1">Phone Number</label>
                            <input type="tel" id="phone" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-ubuntu-green focus:border-ubuntu-green">
                        </div>
                        
                        <div>
                            <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
                            <select id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-ubuntu-green focus:border-ubuntu-green">
                                <option value="">Select a subject</option>
                                <option value="sales">Product Inquiry</option>
                                <option value="consulting">Consulting Services</option>
                                <option value="investment">Investment Opportunities</option>
                                <option value="partnership">Partnership</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                            <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-ubuntu-green focus:border-ubuntu-green"></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-ubuntu-green hover:bg-ubuntu-light-green text-white font-bold py-3 px-6 rounded-lg transition duration-300">Send Message</button>
                    </form>
                </div>
                
                <div>
                    <div class="bg-gray-50 p-8 rounded-lg shadow-sm h-full">
                        <h3 class="text-xl font-bold mb-6 text-ubuntu-darker">Contact Information</h3>
                        
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-ubuntu-green rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fas fa-map-marker-alt"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Headquarters</h4>
                                    <p class="text-gray-600">123 Sustainability Way, Accra, Ghana</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-ubuntu-light-green rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fas fa-phone-alt"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Phone</h4>
                                    <p class="text-gray-600">+233 123 456 789</p>
                                    <p class="text-gray-600">+233 987 654 321</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-ubuntu-lighter-green rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fas fa-envelope"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Email</h4>
                                    <p class="text-gray-600">info@ubuntucs.com</p>
                                    <p class="text-gray-600">sales@ubuntucs.com</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-ubuntu-green rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fas fa-clock"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Working Hours</h4>
                                    <p class="text-gray-600">Monday - Friday: 8:00 AM - 5:00 PM</p>
                                    <p class="text-gray-600">Saturday: 9:00 AM - 1:00 PM</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-semibold text-gray-800 mb-4">Follow Us</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="w-10 h-10 bg-ubuntu-dark hover:bg-ubuntu-darker rounded-full flex items-center justify-center text-white transition duration-300">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="w-10 h-10 bg-ubuntu-dark hover:bg-ubuntu-darker rounded-full flex items-center justify-center text-white transition duration-300">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="w-10 h-10 bg-ubuntu-dark hover:bg-ubuntu-darker rounded-full flex items-center justify-center text-white transition duration-300">
                                    <i class="fab fa-linkedin-in"></i>
                                </a>
                                <a href="#" class="w-10 h-10 bg-ubuntu-dark hover:bg-ubuntu-darker rounded-full flex items-center justify-center text-white transition duration-300">
                                    <i class="fab fa-instagram"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-ubuntu-darker text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-4 gap-8 mb-8">
                <div>
                    <div class="flex items-center mb-4">
                        <div class="w-10 h-10 rounded-full bg-ubuntu-green flex items-center justify-center mr-3">
                            <i class="fas fa-leaf text-white"></i>
                        </div>
                        <span class="text-xl font-bold">Ubuntu<span class="text-ubuntu-light-green">Construction</span></span>
                    </div>
                    <p class="text-gray-300">Building a sustainable future through innovative construction solutions and land restoration.</p>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4 text-ubuntu-light-green">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-300 hover:text-white transition duration-300">Home</a></li>
                        <li><a href="#solutions" class="text-gray-300 hover:text-white transition duration-300">Solutions</a></li>
                        <li><a href="#materials" class="text-gray-300 hover:text-white transition duration-300">Materials</a></li>
                        <li><a href="#impact" class="text-gray-300 hover:text-white transition duration-300">Impact</a></li>
                        <li><a href="#services" class="text-gray-300 hover:text-white transition duration-300">Services</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4 text-ubuntu-light-green">Our Services</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Direct Sales</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Technology Licensing</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Consulting</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Carbon Credits</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Investment</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4 text-ubuntu-light-green">Newsletter</h4>
                    <p class="text-gray-300 mb-4">Subscribe to our newsletter for the latest updates.</p>
                    <div class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 rounded-l-lg focus:outline-none text-gray-800 w-full">
                        <button class="bg-ubuntu-green hover:bg-ubuntu-light-green text-white px-4 py-2 rounded-r-lg transition duration-300">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-700 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-300 mb-4 md:mb-0">© 2023 Ubuntu Construction Solutions. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-300 hover:text-white transition duration-300">Privacy Policy</a>
                    <a href="#" class="text-gray-300 hover:text-white transition duration-300">Terms of Service</a>
                    <a href="#" class="text-gray-300 hover:text-white transition duration-300">Sitemap</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
        
        // Testimonial slider
        const testimonialSlides = document.querySelectorAll('.testimonial-slide');
        const testimonialDots = document.querySelectorAll('.testimonial-dot');
        let currentSlide = 0;
        
        function showSlide(index) {
            testimonialSlides.forEach(slide => slide.classList.remove('active'));
            testimonialDots.forEach(dot => {
                dot.classList.remove('bg-ubuntu-green', 'opacity-100');
                dot.classList.add('bg-gray-300', 'opacity-50');
            });
            
            testimonialSlides[index].classList.add('active');
            testimonialDots[index].classList.remove('bg-gray-300', 'opacity-50');
            testimonialDots[index].classList.add('bg-ubuntu-green', 'opacity-100');
            
            currentSlide = index;
        }
        
        testimonialDots.forEach(dot => {
            dot.addEventListener('click', () => {
                const slideIndex = parseInt(dot.getAttribute('data-slide'));
                showSlide(slideIndex);
            });
        });
        
        // Auto-rotate testimonials
        setInterval(() => {
            let nextSlide = (currentSlide + 1) % testimonialSlides.length;
            showSlide(nextSlide);
        }, 5000);
        
        // Scroll reveal animation
        function animateOnScroll() {
            const elements = document.querySelectorAll('.impact-card, .material-card');
            
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.2;
                
                if (elementPosition < screenPosition) {
                    element.style.opacity = '1';
                    element.style.transform = 'translateY(0)';
                }
            });
        }
        
        // Set initial state for animation
        document.querySelectorAll('.impact-card, .material-card').forEach(element => {
            element.style.opacity = '0';
            element.style.transform = 'translateY(20px)';
            element.style.transition = 'all 0.5s ease';
        });
        
        window.addEventListener('scroll', animateOnScroll);
        window.addEventListener('load', animateOnScroll);
    </script>
</body>
</html>
