# mobilespraytanning
Aurea Mobile Spray Tanning
<script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400;1,600&family=Montserrat:wght@300;400;500;600;700&family=Alex+Brush&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        gold: {
                            100: '#F9F3E5',
                            300: '#E2C889',
                            500: '#C5A059',
                            600: '#B08B43',
                            700: '#8C6C2E',
                        },
                        cream: {
                            50: '#FDFBF7',
                            100: '#FAF6F0',
                            200: '#F2EBDC',
                        },
                        espresso: '#2C2523',
                        sand: '#E6DDD0'
                    },
                    fontFamily: {
                        serif: ['"Cormorant Garamond"', 'serif'],
                        sans: ['Montserrat', 'sans-serif'],
                        script: ['"Alex Brush"', 'cursive'],
                    }
                }
            }
        }
    </script>
    <style>
        .gold-gradient-text {
            background: linear-gradient(135deg, #B08B43 0%, #E2C889 50%, #8C6C2E 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .gold-bg-gradient {
            background: linear-gradient(135deg, #C5A059 0%, #E2C889 50%, #B08B43 100%);
        }
        .hero-bg {
            background-image: linear-gradient(to right, rgba(253, 251, 247, 0.92), rgba(253, 251, 247, 0.75)), url('https://images.unsplash.com/photo-1512290900673-3001886105c3?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }
        .bg-pattern {
            background-color: #FAF6F0;
            background-image: radial-gradient(#C5A059 0.5px, transparent 0.5px), radial-gradient(#C5A059 0.5px, #FAF6F0 0.5px);
            background-size: 20px 20px;
            background-position: 0 0, 10px 10px;
            background-opacity: 0.05;
        }
    </style>
</head>
<body class="bg-cream-50 text-espresso font-sans antialiased selection:bg-gold-500 selection:text-white">

    <!-- Top Announcement Bar -->
    <div class="bg-espresso text-cream-100 text-xs py-2 px-4 text-center tracking-widest uppercase font-medium">
        <span class="inline-block mr-2"><i class="fa-solid fa-sparkles text-gold-300"></i></span> 
        Now Accepting Founding Memberships in Broken Arrow & Greater Tulsa | Limited Spots Available
    </div>

    <!-- Navigation Bar -->
    <nav class="sticky top-0 z-50 bg-cream-50/95 backdrop-blur-md border-b border-gold-500/20 transition-all duration-300 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Brand Logo -->
                <a href="#" class="flex flex-col items-center group">
                    <span class="font-serif text-2xl sm:text-3xl tracking-[0.2em] font-bold text-espresso uppercase group-hover:text-gold-600 transition">Á U R E A</span>
                    <span class="text-[9px] sm:text-[10px] tracking-[0.3em] text-gold-600 uppercase font-medium -mt-1">Mobile Spray Tanning</span>
                </a>

                <!-- Desktop Nav Links -->
                <div class="hidden md:flex items-center space-x-8 text-xs uppercase tracking-widest font-medium">
                    <a href="#about" class="hover:text-gold-600 transition">About</a>
                    <a href="#difference" class="hover:text-gold-600 transition">The Difference</a>
                    <a href="#packages" class="hover:text-gold-600 transition">Packages & Pricing</a>
                    <a href="#memberships" class="hover:text-gold-600 transition">Founding Club</a>
                    <a href="#faq" class="hover:text-gold-600 transition">FAQ</a>
                    <a href="#contact" class="hover:text-gold-600 transition">Contact</a>
                </div>

                <!-- Header CTA Button -->
                <div class="hidden sm:block">
                    <a href="#booking" class="gold-bg-gradient text-white px-6 py-2.5 rounded-full text-xs uppercase tracking-widest font-semibold shadow-md hover:shadow-lg hover:brightness-105 transition transform active:scale-95 inline-block">
                        Book Your Glow
                    </a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-espresso p-2 focus:outline-none" aria-label="Toggle Navigation Menu">
                        <i class="fa-solid fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu Dropdown -->
        <div id="mobile-menu" class="hidden md:hidden bg-cream-100 border-b border-gold-500/20 px-4 pt-2 pb-6 space-y-3 text-center uppercase text-xs tracking-widest">
            <a href="#about" class="block py-2 hover:text-gold-600">About</a>
            <a href="#difference" class="block py-2 hover:text-gold-600">The Difference</a>
            <a href="#packages" class="block py-2 hover:text-gold-600">Packages & Pricing</a>
            <a href="#memberships" class="block py-2 hover:text-gold-600">Founding Club</a>
            <a href="#faq" class="block py-2 hover:text-gold-600">FAQ</a>
            <a href="#contact" class="block py-2 hover:text-gold-600">Contact</a>
            <a href="#booking" class="inline-block mt-2 gold-bg-gradient text-white px-8 py-3 rounded-full text-xs uppercase tracking-widest font-semibold shadow-md">
                Book Your Glow
            </a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative hero-bg py-24 sm:py-32 overflow-hidden border-b border-gold-500/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center sm:text-left relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-7 space-y-6">
                    <div class="inline-flex items-center space-x-2 bg-cream-200/80 px-4 py-1.5 rounded-full border border-gold-500/30">
                        <i class="fa-solid fa-sun text-gold-600 text-xs"></i>
                        <span class="text-[11px] uppercase tracking-widest text-espresso font-semibold">Broken Arrow & Greater Tulsa Mobile Service</span>
                    </div>

                    <h1 class="font-serif text-4xl sm:text-6xl lg:text-7xl font-light text-espresso leading-tight">
                        Golden Glow, <br>
                        <span class="italic font-normal gold-gradient-text">Delivered.</span>
                    </h1>

                    <p class="font-script text-3xl sm:text-4xl text-gold-600 -mt-2">
                        Beauty. Self-Care. Confidence. Anywhere.
                    </p>

                    <p class="text-espresso/80 text-base sm:text-lg max-w-xl font-light leading-relaxed">
                        Experience white-glove luxury mobile spray tanning in the comfort of your own home, venue, or suite. Customized skin-loving formulations designed to nourish your skin while elevating your aura.
                    </p>

                    <div class="pt-4 flex flex-col sm:flex-row items-center justify-center sm:justify-start gap-4">
                        <a href="#booking" class="w-full sm:w-auto gold-bg-gradient text-white px-8 py-4 rounded-full text-xs uppercase tracking-widest font-bold shadow-lg hover:shadow-xl hover:brightness-105 transition transform active:scale-95 text-center">
                            Reserve Appointment
                        </a>
                        <a href="#packages" class="w-full sm:w-auto bg-transparent border border-espresso text-espresso hover:bg-espresso hover:text-white px-8 py-4 rounded-full text-xs uppercase tracking-widest font-medium transition text-center">
                            Explore Packages
                        </a>
                    </div>

                    <!-- Trust indicators -->
                    <div class="pt-8 border-t border-espresso/10 grid grid-cols-3 gap-4 text-center sm:text-left">
                        <div>
                            <div class="font-serif text-2xl font-bold text-gold-700">100%</div>
                            <div class="text-[11px] uppercase tracking-wider text-espresso/70">Custom Shade Match</div>
                        </div>
                        <div>
                            <div class="font-serif text-2xl font-bold text-gold-700">Zero</div>
                            <div class="text-[11px] uppercase tracking-wider text-espresso/70">UV Ray Exposure</div>
                        </div>
                        <div>
                            <div class="font-serif text-2xl font-bold text-gold-700">Mobile</div>
                            <div class="text-[11px] uppercase tracking-wider text-espresso/70">We Travel To You</div>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-5 relative">
                    <div class="relative mx-auto max-w-md lg:max-w-none">
                        <div class="aspect-[4/5] rounded-t-full rounded-b-2xl overflow-hidden border-8 border-cream-100 shadow-2xl relative">
                            <img src="https://images.unsplash.com/photo-1540555700478-4be289fbecef?auto=format&fit=crop&w=800&q=80" alt="Luxury Tanning Glow" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-espresso/40 via-transparent to-transparent"></div>
                            <div class="absolute bottom-6 left-6 right-6 text-white text-center p-4 bg-cream-50/20 backdrop-blur-md rounded-xl border border-white/30">
                                <span class="font-script text-2xl block text-gold-300">Self-Care Looks Good On You</span>
                                <span class="text-[10px] uppercase tracking-widest font-medium">Aurea Skin-Loving Ritual</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Brand Story & Pronunciation -->
    <section id="about" class="py-20 bg-cream-100 relative border-b border-gold-500/20">
        <div class="max-w-4xl mx-auto px-4 text-center space-y-6">
            <span class="text-xs uppercase tracking-[0.3em] text-gold-600 font-semibold block">The Meaning Behind The Name</span>
            <h2 class="font-serif text-3xl sm:text-5xl font-light text-espresso">
                Á U R E A <span class="text-lg font-sans font-normal text-gold-600 block sm:inline italic">/AW-RAY-UH/</span>
            </h2>
            <p class="font-serif text-xl italic text-gold-700">"Golden" — Latin</p>
            
            <div class="w-16 h-0.5 bg-gold-500 mx-auto my-4"></div>

            <p class="text-espresso/80 text-base sm:text-lg leading-relaxed font-light">
                Aurea is inspired by the Latin word for <strong>"golden."</strong> More than just a shade, it represents a feeling: sun-kissed warmth, radiant health, conscious self-care, and the effortless confidence that comes from feeling your absolute best.
            </p>
            <p class="text-espresso/80 text-base sm:text-lg leading-relaxed font-light">
                Its sound echoes the word <em>aura</em>—the unique energy you carry into every room. Because a true glow isn't just what you see on the outside; it's how you feel on the inside.
            </p>
        </div>
    </section>

    <!-- The Aurea Difference / Features -->
    <section id="difference" class="py-24 bg-cream-50 border-b border-gold-500/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-3">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-600 font-semibold">Elevated Self-Care</span>
                <h2 class="font-serif text-3xl sm:text-5xl text-espresso font-light">More Than A Spray Tan. A Ritual.</h2>
                <p class="text-espresso/70 text-sm sm:text-base font-light">A spray tan shouldn't feel like a beauty chore—it should feel like luxury self-care.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Feature 1 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-leaf"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Skin-Loving Ingredients</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        Infused with rich botanicals, aloe vera, coconut water, hyaluronic acid, and vitamins C & E to hydrate and nourish skin deeply while developing.
                    </p>
                </div>

                <!-- Feature 2 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-sliders"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Customized Color Matching</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        Every glow is tailored individually to your specific skin tone, undertones, upcoming occasion, and personal bronzing preference. Never orange or brassy.
                    </p>
                </div>

                <!-- Feature 3 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-house-chimney-window"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Mobile Convenience</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        White-glove luxury service delivered directly to your doorstep, hotel, or bridal venue across Broken Arrow, Tulsa, Bixby, and surrounding areas.
                    </p>
                </div>

                <!-- Feature 4 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-shield-halved"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Zero UV Damage</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        Achieve a rich, radiant bronzed complexion without exposing your skin to harmful UV radiation, aging rays, or tanning bed burns.
                    </p>
                </div>

                <!-- Feature 5 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-spray-can-sparkles"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Mess-Free Setup</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        We bring a professional pop-up pop tent, overspray extraction filtration, and protective gear. Your home remains 100% spotless.
                    </p>
                </div>

                <!-- Feature 6 -->
                <div class="bg-cream-100 p-8 rounded-2xl border border-gold-500/20 shadow-sm hover:shadow-md transition">
                    <div class="w-12 h-12 rounded-full bg-gold-100 flex items-center justify-center text-gold-600 mb-6 text-xl">
                        <i class="fa-solid fa-heart"></i>
                    </div>
                    <h3 class="font-serif text-2xl text-espresso mb-3">Confidence Included</h3>
                    <p class="text-espresso/70 text-sm leading-relaxed font-light">
                        Whether it's date night, a major photoshoot, vacation, wedding day, or a weekly refresh, you leave feeling empowered and radiant.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Packages & Pricing -->
    <section id="packages" class="py-24 bg-cream-100 border-b border-gold-500/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-3">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-600 font-semibold">Invest In Your Glow</span>
                <h2 class="font-serif text-3xl sm:text-5xl text-espresso font-light">Glow Packages & Bundles</h2>
                <p class="text-espresso/70 text-sm sm:text-base font-light">More glows. More savings. A more radiant you.</p>
            </div>

            <!-- Pricing Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 items-stretch">
                <!-- Single Glow -->
                <div class="bg-cream-50 rounded-2xl p-8 border border-gold-500/30 flex flex-col justify-between hover:border-gold-500 transition shadow-sm">
                    <div>
                        <div class="text-[10px] uppercase tracking-widest text-gold-600 font-semibold mb-2">Single Session</div>
                        <h3 class="font-serif text-2xl text-espresso font-medium">Custom Mobile Glow</h3>
                        <div class="my-6">
                            <span class="font-serif text-4xl font-bold text-espresso">$59</span>
                            <span class="text-xs text-espresso/60 block mt-1">Full body custom color application</span>
                        </div>
                        <ul class="space-y-3 text-xs text-espresso/80 font-light mb-8">
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Custom undertone solution</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Mobile travel included</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Hydrating prep spray</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Finishing powder treatment</li>
                        </ul>
                    </div>
                    <a href="#booking" class="w-full text-center py-3 border border-gold-600 text-gold-700 hover:bg-gold-600 hover:text-white rounded-full text-xs uppercase tracking-widest font-semibold transition">Select Option</a>
                </div>

                <!-- Golden Trio -->
                <div class="bg-cream-50 rounded-2xl p-8 border border-gold-500/30 flex flex-col justify-between hover:border-gold-500 transition shadow-sm relative">
                    <div>
                        <div class="text-[10px] uppercase tracking-widest text-gold-600 font-semibold mb-2">Save $12</div>
                        <h3 class="font-serif text-2xl text-espresso font-medium">Golden Trio Pack</h3>
                        <div class="my-6">
                            <span class="font-serif text-4xl font-bold text-espresso">$165</span>
                            <span class="text-xs text-espresso/60 block mt-1">$55 per tan (3 Spray Tans)</span>
                        </div>
                        <ul class="space-y-3 text-xs text-espresso/80 font-light mb-8">
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> 3 Custom Mobile Tans</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Save $12 off regular rate</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Perfect for events & vacations</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> 12-Month expiration</li>
                        </ul>
                    </div>
                    <a href="#booking" class="w-full text-center py-3 border border-gold-600 text-gold-700 hover:bg-gold-600 hover:text-white rounded-full text-xs uppercase tracking-widest font-semibold transition">Select Option</a>
                </div>

                <!-- Radiance Collection (Most Popular) -->
                <div class="bg-cream-50 rounded-2xl p-8 border-2 border-gold-500 flex flex-col justify-between shadow-lg relative transform lg:-translate-y-2">
                    <div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-gold-600 text-white text-[9px] uppercase tracking-widest px-4 py-1 rounded-full font-bold">Most Popular</div>
                    <div>
                        <div class="text-[10px] uppercase tracking-widest text-gold-600 font-semibold mb-2">Save $30</div>
                        <h3 class="font-serif text-2xl text-espresso font-medium">Radiance Collection</h3>
                        <div class="my-6">
                            <span class="font-serif text-4xl font-bold text-espresso">$265</span>
                            <span class="text-xs text-espresso/60 block mt-1">$53 per tan (5 Spray Tans)</span>
                        </div>
                        <ul class="space-y-3 text-xs text-espresso/80 font-light mb-8">
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> 5 Custom Mobile Tans</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Save $30 off regular rate</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Regular monthly maintenance</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Priority scheduling perk</li>
                        </ul>
                    </div>
                    <a href="#booking" class="w-full text-center py-3 gold-bg-gradient text-white rounded-full text-xs uppercase tracking-widest font-bold shadow-md hover:brightness-105 transition">Select Option</a>
                </div>

                <!-- Signature Glow Society -->
                <div class="bg-cream-50 rounded-2xl p-8 border border-gold-500/30 flex flex-col justify-between hover:border-gold-500 transition shadow-sm">
                    <div>
                        <div class="text-[10px] uppercase tracking-widest text-gold-600 font-semibold mb-2">Save $81</div>
                        <h3 class="font-serif text-2xl text-espresso font-medium">Signature Glow Society</h3>
                        <div class="my-6">
                            <span class="font-serif text-4xl font-bold text-espresso">$450</span>
                            <span class="text-xs text-espresso/60 block mt-1">$50 per tan (9 Spray Tans)</span>
                        </div>
                        <ul class="space-y-3 text-xs text-espresso/80 font-light mb-8">
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> 9 Custom Mobile Tans</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Best value ($81 total savings)</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Ideal for brides & VIP clients</li>
                            <li class="flex items-center"><i class="fa-solid fa-check text-gold-600 mr-2"></i> Shareable with 1 friend</li>
                        </ul>
                    </div>
                    <a href="#booking" class="w-full text-center py-3 border border-gold-600 text-gold-700 hover:bg-gold-600 hover:text-white rounded-full text-xs uppercase tracking-widest font-semibold transition">Select Option</a>
                </div>
            </div>

            <!-- Group & Event Callout -->
            <div class="mt-12 bg-espresso text-cream-100 rounded-2xl p-8 sm:p-10 flex flex-col md:flex-row items-center justify-between gap-6 shadow-xl">
                <div class="space-y-2 text-center md:text-left">
                    <span class="text-gold-300 text-xs uppercase tracking-widest font-semibold">Bridal Parties & Special Events</span>
                    <h3 class="font-serif text-2xl sm:text-3xl text-cream-50">Hosting a Spray Tan Party or Wedding?</h3>
                    <p class="text-cream-200/70 text-xs sm:text-sm font-light">Host gets a complimentary glow when booking groups of 5 or more in Broken Arrow or Tulsa.</p>
                </div>
                <a href="#contact" class="bg-gold-500 hover:bg-gold-600 text-white px-8 py-3.5 rounded-full text-xs uppercase tracking-widest font-bold transition whitespace-nowrap">
                    Inquire For Group Rates
                </a>
            </div>
        </div>
    </section>

    <!-- Founding Memberships VIP Banner -->
    <section id="memberships" class="py-20 bg-espresso text-cream-50 relative overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div class="space-y-6">
                    <span class="text-gold-300 text-xs uppercase tracking-[0.3em] font-bold">Limited Availability</span>
                    <h2 class="font-serif text-4xl sm:text-5xl font-light">
                        Become An ÁUREA <br>
                        <span class="italic font-normal text-gold-300">Founding Member</span>
                    </h2>
                    <p class="text-cream-100/80 text-sm sm:text-base font-light leading-relaxed">
                        Be part of something radiant from the very beginning. Lock in exclusive founding rates, VIP appointment slots, and complimentary skin upgrades before enrollment closes.
                    </p>

                    <div class="grid grid-cols-2 gap-4 pt-2">
                        <div class="border border-gold-500/30 p-4 rounded-xl bg-cream-50/5">
                            <i class="fa-solid fa-gem text-gold-300 mb-2"></i>
                            <h4 class="font-serif text-lg">Exclusive Rates</h4>
                            <p class="text-xs text-cream-200/60 font-light">Lock in founding member pricing for life.</p>
                        </div>
                        <div class="border border-gold-500/30 p-4 rounded-xl bg-cream-50/5">
                            <i class="fa-solid fa-calendar-check text-gold-300 mb-2"></i>
                            <h4 class="font-serif text-lg">Priority Booking</h4>
                            <p class="text-xs text-cream-200/60 font-light">First access to prime evening & weekend slots.</p>
                        </div>
                    </div>

                    <a href="#booking" class="inline-block gold-bg-gradient text-white px-8 py-4 rounded-full text-xs uppercase tracking-widest font-bold shadow-lg hover:brightness-105 transition">
                        Join The Founding List
                    </a>
                </div>

                <div class="bg-cream-100 text-espresso p-8 sm:p-10 rounded-2xl shadow-2xl space-y-6 border border-gold-500/40">
                    <div class="text-center space-y-2 border-b border-gold-500/20 pb-6">
                        <h3 class="font-serif text-2xl font-bold uppercase tracking-wider">Founding VIP Glow Membership</h3>
                        <p class="text-gold-600 font-serif italic text-lg">$99 / month</p>
                    </div>
                    <ul class="space-y-4 text-xs font-light">
                        <li class="flex items-center"><i class="fa-solid fa-sparkles text-gold-600 mr-3 text-base"></i> <strong>2 Custom Mobile Tans</strong> included per month ($118 value)</li>
                        <li class="flex items-center"><i class="fa-solid fa-sparkles text-gold-600 mr-3 text-base"></i> <strong>Free Hydration Skin Boosters</strong> with every appointment</li>
                        <li class="flex items-center"><i class="fa-solid fa-sparkles text-gold-600 mr-3 text-base"></i> <strong>15% Off</strong> all additional spray tans & retail products</li>
                        <li class="flex items-center"><i class="fa-solid fa-sparkles text-gold-600 mr-3 text-base"></i> Rollover unused spray tans for up to 60 days</li>
                        <li class="flex items-center"><i class="fa-solid fa-sparkles text-gold-600 mr-3 text-base"></i> No long-term contracts; cancel anytime with 30 days notice</li>
                    </ul>
                    <a href="#booking" class="block w-full text-center bg-espresso text-cream-50 py-3 rounded-full text-xs uppercase tracking-widest font-semibold hover:bg-gold-600 transition">
                        Claim Founding Membership
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Vagaro Booking Portal Section -->
    <section id="booking" class="py-24 bg-cream-50 border-b border-gold-500/20">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12 space-y-3">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-600 font-semibold">Reserve Your Appointment</span>
                <h2 class="font-serif text-3xl sm:text-5xl text-espresso font-light">Online Booking Portal</h2>
                <p class="text-espresso/70 text-sm font-light">Select your service, choose your preferred time, and we'll bring the luxury glow directly to you.</p>
            </div>

            <!-- Booking Frame Container / Vagaro Integration Placeholder -->
            <div class="bg-cream-100 p-6 sm:p-10 rounded-3xl border border-gold-500/30 shadow-xl">
                <!-- Interactive Simulated Booking Widget for smooth UI experience -->
                <div id="vagaro-booking-sim" class="space-y-8">
                    <!-- Step Indicator -->
                    <div class="flex justify-between items-center text-xs border-b border-gold-500/20 pb-4 font-medium uppercase tracking-wider">
                        <span class="text-gold-700 font-bold">1. Select Service</span>
                        <span class="text-espresso/40">2. Address & Time</span>
                        <span class="text-espresso/40">3. Confirmation</span>
                    </div>

                    <!-- Step 1 Form -->
                    <div class="space-y-6">
                        <div>
                            <label class="block text-xs uppercase tracking-wider text-espresso font-semibold mb-2">Choose Treatment / Package</label>
                            <select id="service-select" class="w-full bg-cream-50 border border-gold-500/40 rounded-xl p-3 text-sm text-espresso focus:outline-none focus:border-gold-600">
                                <option value="single">Single Custom Mobile Glow ($59)</option>
                                <option value="trio">Golden Trio Pack - 3 Tans ($165)</option>
                                <option value="radiance">Radiance Collection - 5 Tans ($265)</option>
                                <option value="society">Signature Glow Society - 9 Tans ($450)</option>
                                <option value="founding">Founding VIP Membership ($99/mo)</option>
                                <option value="party">Group / Bridal Party Booking</option>
                            </select>
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-xs uppercase tracking-wider text-espresso font-semibold mb-2">Your Location / City</label>
                                <select class="w-full bg-cream-50 border border-gold-500/40 rounded-xl p-3 text-sm text-espresso focus:outline-none focus:border-gold-600">
                                    <option value="ba">Broken Arrow, OK</option>
                                    <option value="tulsa">Tulsa, OK</option>
                                    <option value="bixby">Bixby, OK</option>
                                    <option value="jenks">Jenks, OK</option>
                                    <option value="owasso">Owasso, OK</option>
                                    <option value="other">Other Surrounding Area</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-xs uppercase tracking-wider text-espresso font-semibold mb-2">Preferred Date</label>
                                <input type="date" class="w-full bg-cream-50 border border-gold-500/40 rounded-xl p-3 text-sm text-espresso focus:outline-none focus:border-gold-600">
                            </div>
                        </div>

                        <div>
                            <label class="block text-xs uppercase tracking-wider text-espresso font-semibold mb-2">Special Notes or Skin Concerns</label>
                            <textarea rows="3" placeholder="Upcoming wedding, sensitive skin, rapid tan request..." class="w-full bg-cream-50 border border-gold-500/40 rounded-xl p-3 text-sm text-espresso focus:outline-none focus:border-gold-600"></textarea>
                        </div>

                        <button type="button" onclick="handleBookingSubmit()" class="w-full gold-bg-gradient text-white py-4 rounded-full text-xs uppercase tracking-widest font-bold shadow-md hover:brightness-105 transition">
                            Proceed To Booking System
                        </button>
                    </div>

                    <!-- Direct Vagaro Link Backup -->
                    <div class="text-center pt-4 border-t border-gold-500/20">
                        <p class="text-xs text-espresso/60">
                            Prefer booking directly through Vagaro? 
                            <a href="https://www.vagaro.com" target="_blank" class="text-gold-700 underline font-semibold hover:text-gold-800">Click Here to Open Vagaro Portal</a>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Accordion -->
    <section id="faq" class="py-24 bg-cream-100 border-b border-gold-500/20">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-600 font-semibold">Glow Preparation & Care</span>
                <h2 class="font-serif text-3xl sm:text-5xl text-espresso font-light">Frequently Asked Questions</h2>
            </div>

            <div class="space-y-4">
                <!-- Q1 -->
                <div class="bg-cream-50 rounded-2xl border border-gold-500/20 overflow-hidden">
                    <button class="faq-btn w-full p-6 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-serif text-lg text-espresso font-medium">How should I prepare my skin before my mobile spray tan?</span>
                        <i class="fa-solid fa-chevron-down text-gold-600 transition-transform duration-200"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 text-xs sm:text-sm text-espresso/70 font-light leading-relaxed">
                        Exfoliate 18-24 hours prior to your appointment using a oil-free scrub or exfoliating mitt. Complete all hair removal, manicures, and pedicures beforehand. Arrive with clean skin—free of lotions, perfumes, deodorant, or makeup.
                    </div>
                </div>

                <!-- Q2 -->
                <div class="bg-cream-50 rounded-2xl border border-gold-500/20 overflow-hidden">
                    <button class="faq-btn w-full p-6 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-serif text-lg text-espresso font-medium">What should I wear during and after the appointment?</span>
                        <i class="fa-solid fa-chevron-down text-gold-600 transition-transform duration-200"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 text-xs sm:text-sm text-espresso/70 font-light leading-relaxed">
                        During the tan, wear whatever makes you feel comfortable—swimwear, dark underwear, or tan nude lines. After your tan, wear loose-fitting, dark clothing and flip-flops while the color develops to prevent creasing.
                    </div>
                </div>

                <!-- Q3 -->
                <div class="bg-cream-50 rounded-2xl border border-gold-500/20 overflow-hidden">
                    <button class="faq-btn w-full p-6 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-serif text-lg text-espresso font-medium">How long will my Aurea tan last?</span>
                        <i class="fa-solid fa-chevron-down text-gold-600 transition-transform duration-200"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 text-xs sm:text-sm text-espresso/70 font-light leading-relaxed">
                        With proper prep and daily hydration, your custom spray tan will last 7 to 10 days. Moisture is key—we recommend applying oil-free moisturizer daily to keep your skin glowing evenly.
                    </div>
                </div>

                <!-- Q4 -->
                <div class="bg-cream-50 rounded-2xl border border-gold-500/20 overflow-hidden">
                    <button class="faq-btn w-full p-6 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-serif text-lg text-espresso font-medium">Will my house or furniture get dirty?</span>
                        <i class="fa-solid fa-chevron-down text-gold-600 transition-transform duration-200"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 text-xs sm:text-sm text-espresso/70 font-light leading-relaxed">
                        Not at all! We bring a full mobile setup including a clean pop-up extraction enclosure and floor mats. All spray tan solution is contained entirely within our tent.
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer & Contact / Business Verification Info -->
    <footer id="contact" class="bg-espresso text-cream-100 py-16 border-t border-gold-500/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-10 border-b border-cream-100/10 pb-12">
                <!-- Col 1: Brand Info -->
                <div class="space-y-4 md:col-span-1">
                    <a href="#" class="inline-block">
                        <span class="font-serif text-2xl tracking-[0.2em] font-bold text-cream-50 uppercase">Á U R E A</span>
                        <span class="text-[9px] tracking-[0.3em] text-gold-300 uppercase block">Mobile Spray Tanning</span>
                    </a>
                    <p class="text-xs text-cream-200/70 font-light leading-relaxed">
                        Luxury mobile spray tanning service operating out of Broken Arrow, Oklahoma and serving the Greater Tulsa Metropolitan area.
                    </p>
                </div>

                <!-- Col 2: Quick Links -->
                <div class="space-y-3 text-xs">
                    <h4 class="font-serif text-gold-300 text-sm uppercase tracking-wider">Quick Links</h4>
                    <ul class="space-y-2 text-cream-200/70 font-light">
                        <li><a href="#about" class="hover:text-gold-300">About Aurea</a></li>
                        <li><a href="#packages" class="hover:text-gold-300">Glow Packages</a></li>
                        <li><a href="#memberships" class="hover:text-gold-300">Founding Club</a></li>
                        <li><a href="#booking" class="hover:text-gold-300">Book Appointment</a></li>
                    </ul>
                </div>

                <!-- Col 3: Service Areas -->
                <div class="space-y-3 text-xs">
                    <h4 class="font-serif text-gold-300 text-sm uppercase tracking-wider">Service Areas</h4>
                    <ul class="space-y-1 text-cream-200/70 font-light">
                        <li>Broken Arrow, OK (HQ)</li>
                        <li>Tulsa, OK</li>
                        <li>Bixby & Jenks, OK</li>
                        <li>Owasso & Coweta, OK</li>
                    </ul>
                </div>

                <!-- Col 4: Business & Verification Details -->
                <div class="space-y-3 text-xs">
                    <h4 class="font-serif text-gold-300 text-sm uppercase tracking-wider">Contact & Business Info</h4>
                    <p class="text-cream-200/70 font-light"><i class="fa-solid fa-envelope text-gold-300 mr-2"></i> hello@aureaspraytanning.com</p>
                    <p class="text-cream-200/70 font-light"><i class="fa-solid fa-phone text-gold-300 mr-2"></i> (918) 555-GLOW</p>
                    <p class="text-cream-200/70 font-light"><i class="fa-solid fa-location-dot text-gold-300 mr-2"></i> Broken Arrow, OK 74012</p>
                    
                    <div class="flex space-x-4 pt-2 text-gold-300 text-base">
                        <a href="#" aria-label="Instagram"><i class="fa-brands fa-instagram hover:text-white transition"></i></a>
                        <a href="#" aria-label="Facebook"><i class="fa-brands fa-facebook hover:text-white transition"></i></a>
                        <a href="#" aria-label="TikTok"><i class="fa-brands fa-tiktok hover:text-white transition"></i></a>
                    </div>
                </div>
            </div>

            <div class="pt-8 flex flex-col sm:flex-row justify-between items-center text-[10px] text-cream-200/50 space-y-4 sm:space-y-0">
                <p>&copy; 2026 Áurea Mobile Spray Tanning. All Rights Reserved. Broken Arrow, OK.</p>
                <p class="tracking-widest uppercase">Golden Glow, Delivered.</p>
            </div>
        </div>
    </footer>

    <!-- Notification Modal for Booking Action -->
    <div id="booking-modal" class="fixed inset-0 bg-espresso/80 backdrop-blur-sm z-50 flex items-center justify-center hidden p-4">
        <div class="bg-cream-50 rounded-2xl max-w-md w-full p-8 border border-gold-500/40 shadow-2xl text-center space-y-4">
            <div class="w-16 h-16 bg-gold-100 rounded-full flex items-center justify-center text-gold-600 text-2xl mx-auto">
                <i class="fa-solid fa-check"></i>
            </div>
            <h3 class="font-serif text-2xl text-espresso">Selection Received</h3>
            <p class="text-xs text-espresso/70 leading-relaxed font-light">
                Your luxury treatment selection has been logged. Redirecting to our Vagaro booking portal to select your precise appointment slot and finalize details...
            </p>
            <button onclick="closeModal()" class="w-full gold-bg-gradient text-white py-3 rounded-full text-xs uppercase tracking-widest font-bold">
                Continue to Vagaro
            </button>
        </div>
    </div>

    <!-- JavaScript Interactions -->
    <script>
        // Mobile Navigation Toggle
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // FAQ Accordion Toggle
        const faqBtns = document.querySelectorAll('.faq-btn');
        faqBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                const content = btn.nextElementSibling;
                const icon = btn.querySelector('i');
                
                content.classList.toggle('hidden');
                icon.classList.toggle('rotate-180');
            });
        });

        // Booking Modal Handle
        function handleBookingSubmit() {
            document.getElementById('booking-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('booking-modal').classList.add('hidden');
            // Redirect to Vagaro portal or direct booking URL
            window.open('https://www.vagaro.com', '_blank');
        }
    </script>
</body>
</html>
