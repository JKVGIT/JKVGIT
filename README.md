<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jitendra Verma · Full Stack & React Native</title>
    <!-- Tailwind + Fancy Font + Animation base -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome 6 (free) for extra polish -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Framer Motion (via ESM + React) – but we'll do a lightweight approximate animation with simple CSS + AOS flavour -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700&display=swap');
        body { font-family: 'Inter', sans-serif; background: #0a0c10; scroll-behavior: smooth; }
        .glow-text { text-shadow: 0 0 10px rgba(0,255,255,0.5); }
        .card-shine {
            background: linear-gradient(145deg, #1e2128, #13161c);
            box-shadow: 0 25px 40px -15px rgba(0,255,200,0.15);
            transition: all 0.3s ease;
        }
        .card-shine:hover {
            box-shadow: 0 30px 50px -15px #00e0ff80;
            transform: translateY(-5px);
        }
        .icon-pulse {
            animation: softPulse 3s infinite;
        }
        @keyframes softPulse {
            0% { filter: drop-shadow(0 0 2px #00ffe1); }
            50% { filter: drop-shadow(0 0 10px #4df0ff); }
            100% { filter: drop-shadow(0 0 2px #00ffe1); }
        }
        .skill-icon {
            transition: transform 0.2s;
        }
        .skill-icon:hover {
            transform: scale(1.15) rotate(2deg);
        }
        .bg-grid {
            background-image: radial-gradient(#2a2f3a 1px, transparent 1px);
            background-size: 40px 40px;
        }
    </style>
</head>
<body class="bg-[#0a0c10] text-gray-200 flex items-center justify-center min-h-screen p-4 md:p-8">

<!-- main card container with responsive max width and futuristic feel -->
<div class="max-w-4xl w-full relative z-10" data-aos="fade-up" data-aos-duration="700">

    <!-- header section with wave hand and animated gradient border -->
    <div class="card-shine rounded-3xl p-8 md:p-10 border border-cyan-500/20 relative overflow-hidden" data-aos="zoom-in" data-aos-delay="100">
        <div class="absolute inset-0 bg-grid opacity-20"></div>
        <div class="relative z-10">
            <div class="flex flex-col md:flex-row md:items-center md:justify-between gap-4">
                <div>
                    <span class="inline-flex items-center gap-2 bg-cyan-500/10 text-cyan-300 px-4 py-1.5 rounded-full text-sm font-medium border border-cyan-400/30 mb-4">
                        <i class="fas fa-code text-cyan-300"></i> full stack · react native
                    </span>
                    <h1 class="text-4xl md:text-5xl font-bold flex items-center gap-3 tracking-tight">
                        JITENDRA VERMA
                        <span class="text-5xl origin-bottom-right inline-block animate-bounce" style="animation-duration: 1.5s;">👋</span>
                    </h1>
                    <p class="text-xl text-gray-300 mt-3 flex items-center gap-2">
                        <i class="fas fa-rocket text-cyan-400 text-2xl icon-pulse"></i>
                        <span>Building production-grade business apps with <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-300 to-teal-300 font-semibold">React, Django, and Flutter</span></span>
                    </p>
                </div>
                <!-- avatar-like placeholder with tech symbols (iconic) -->
                <div class="flex gap-3 self-start md:self-center text-4xl text-cyan-300/80">
                    <i class="fab fa-react fa-fw animate-spin-slow" style="animation: spin 8s linear infinite;"></i>
                    <i class="fab fa-python fa-fw"></i>
                    <i class="fas fa-database fa-fw"></i>
                    <i class="fab fa-php fa-fw"></i>
                </div>
            </div>

            <!-- about me section as compact micro cards -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mt-10">
                <div class="bg-[#1c212a] p-4 rounded-xl border border-gray-700 flex items-center gap-3 hover:border-cyan-500/50 transition" data-aos="fade-right" data-aos-delay="150">
                    <i class="fas fa-bolt text-yellow-400 text-xl"></i>
                    <div><span class="text-gray-400 text-sm">currently</span><br><span class="font-medium">Production level apps</span></div>
                </div>
                <div class="bg-[#1c212a] p-4 rounded-xl border border-gray-700 flex items-center gap-3 hover:border-cyan-500/50 transition" data-aos="fade-right" data-aos-delay="200">
                    <i class="fas fa-graduation-cap text-green-400 text-xl"></i>
                    <div><span class="text-gray-400 text-sm">learning</span><br><span class="font-medium">Advanced Django</span></div>
                </div>
                <div class="bg-[#1c212a] p-4 rounded-xl border border-gray-700 flex items-center gap-3 hover:border-cyan-500/50 transition" data-aos="fade-left" data-aos-delay="250">
                    <i class="fas fa-comment-dots text-sky-400 text-xl"></i>
                    <div><span class="text-gray-400 text-sm">ask me about</span><br><span class="font-medium">React, PHP, MySQL</span></div>
                </div>
                <div class="bg-[#1c212a] p-4 rounded-xl border border-gray-700 flex items-center gap-3 hover:border-cyan-500/50 transition" data-aos="fade-left" data-aos-delay="300">
                    <i class="fas fa-bullseye text-purple-400 text-xl"></i>
                    <div><span class="text-gray-400 text-sm">focus</span><br><span class="font-medium">real‑world problems</span></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Tech Stack with animated icons using skillicons + custom overlay pulse -->
    <div class="mt-8 card-shine rounded-3xl p-8 border border-gray-800 relative" data-aos="fade-up" data-aos-delay="200">
        <h2 class="text-2xl font-semibold mb-6 flex items-center gap-3"><i class="fas fa-cubes text-cyan-400"></i> <span class="bg-gradient-to-r from-white to-gray-300 bg-clip-text text-transparent">Tech Stack</span></h2>
        <!-- using skillicons.dev for crisp icons (they are interactive by themselves) -->
        <div class="flex flex-wrap items-center justify-center gap-4 md:gap-6 py-4">
            <img src="https://skillicons.dev/icons?i=react,nodejs,django,php,mysql,js,html,css,flutter,git&perline=5" alt="tech stack icons" class="max-w-full h-auto skill-icon" style="filter: drop-shadow(0 0 8px #00b8b0);" />
        </div>
        <p class="text-gray-400 text-sm mt-4 text-center flex gap-2 items-center justify-center"><i class="fas fa-crown text-yellow-500"></i> daily drivers — production ready <i class="fas fa-crown text-yellow-500"></i></p>
    </div>

    <!-- GitHub Stats with twin cards: stats + top langs -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-8">
        <!-- github stats card -->
        <div class="card-shine rounded-3xl p-6 border border-gray-800 flex flex-col" data-aos="flip-left" data-aos-delay="250">
            <div class="flex items-center gap-2 text-xl font-medium mb-4"><i class="fab fa-github text-2xl"></i> <span>GitHub stats</span></div>
            <div class="flex-1 flex items-center justify-center p-2 bg-[#11141c] rounded-xl">
                <!-- we embed an actual stats image but with a smooth fallback using placeholder. For realism I'll generate with the username -->
                <img src="https://github-readme-stats.vercel.app/api?username=BSDeveloper263&show_icons=true&theme=radical&border_radius=12&hide_border=true&bg_color=0d1117" alt="github stats" class="rounded-lg w-full" />
            </div>
        </div>
        <!-- top languages card -->
        <div class="card-shine rounded-3xl p-6 border border-gray-800 flex flex-col" data-aos="flip-right" data-aos-delay="300">
            <div class="flex items-center gap-2 text-xl font-medium mb-4"><i class="fas fa-chart-pie text-2xl text-green-300"></i> <span>top languages</span></div>
            <div class="flex-1 flex items-center justify-center p-2 bg-[#11141c] rounded-xl">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=BSDeveloper263&layout=compact&theme=radical&border_radius=12&hide_border=true&bg_color=0d1117" alt="top languages" class="rounded-lg w-full" />
            </div>
        </div>
    </div>

    <!-- Current Focus + extra touch: project categories with icons & visual indicators -->
    <div class="mt-8 card-shine rounded-3xl p-8 border border-cyan-500/20" data-aos="fade-up" data-aos-delay="300">
        <h2 class="text-2xl font-semibold mb-4 flex items-center gap-2"><i class="fas fa-fire-flame text-orange-400"></i> 🔥 current focus</h2>
        <div class="grid grid-cols-1 sm:grid-cols-3 gap-5 text-center md:text-left">
            <div class="bg-[#1a1f2a] p-5 rounded-2xl border border-gray-700 hover:border-cyan-500/70 transition-all" data-aos="zoom-in" data-aos-delay="350">
                <i class="fas fa-mobile-screen-button text-4xl text-cyan-300 mb-3"></i>
                <h3 class="font-semibold text-lg">Cross‑platform apps</h3>
                <p class="text-sm text-gray-400">React Native & Flutter</p>
                <span class="inline-block w-12 h-1 bg-cyan-500/50 rounded-full mt-2"></span>
            </div>
            <div class="bg-[#1a1f2a] p-5 rounded-2xl border border-gray-700 hover:border-cyan-500/70 transition-all" data-aos="zoom-in" data-aos-delay="400">
                <i class="fas fa-briefcase text-4xl text-teal-300 mb-3"></i>
                <h3 class="font-semibold text-lg">Business web apps</h3>
                <p class="text-sm text-gray-400">Django, React, PHP</p>
                <span class="inline-block w-12 h-1 bg-teal-500/50 rounded-full mt-2"></span>
            </div>
            <div class="bg-[#1a1f2a] p-5 rounded-2xl border border-gray-700 hover:border-cyan-500/70 transition-all" data-aos="zoom-in" data-aos-delay="450">
                <i class="fas fa-microchip text-4xl text-purple-300 mb-3"></i>
                <h3 class="font-semibold text-lg">Backend optimization</h3>
                <p class="text-sm text-gray-400">DB tuning, Django perf</p>
                <span class="inline-block w-12 h-1 bg-purple-500/50 rounded-full mt-2"></span>
            </div>
        </div>
        <!-- motivational line -->
        <div class="mt-8 text-center text-sm text-gray-500 flex items-center justify-center gap-2 border-t border-gray-800 pt-4">
            <i class="fas fa-star text-yellow-500 animate-ping" style="animation-iteration-count: 2;"></i>
            <span>From Jitendra Verma — code, create, scale</span>
            <i class="fas fa-star text-yellow-500 animate-ping" style="animation-iteration-count: 2;"></i>
        </div>
    </div>

    <!-- footer note "⭐ From Jitendra Verma" with some icons -->
    <div class="mt-6 flex flex-wrap items-center justify-between text-sm text-gray-400 border-t border-gray-800 pt-4">
        <div class="flex gap-3">
            <i class="fab fa-github hover:text-white transition"></i>
            <i class="fab fa-linkedin hover:text-white transition"></i>
            <i class="fab fa-twitter hover:text-white transition"></i>
        </div>
        <div class="flex gap-2">
            <span>⭐</span> <span class="tracking-wide">From Jitendra Verma · Full Stack & React Native</span>
        </div>
    </div>

    <!-- small watermark animation (just for delight) -->
    <div class="absolute -bottom-6 right-6 opacity-10 text-7xl pointer-events-none select-none hidden md:block">
        <i class="fas fa-brackets-curly"></i>
    </div>
</div>

<!-- AOS init for scroll animations (even though minimal scroll, they run on load) -->
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
    AOS.init({
        once: true,
        duration: 600,
        easing: 'ease-out-sine',
    });
    // additional micro interaction: the wave hand can pulse 
    const hand = document.querySelector('h1 span');
    if(hand) {
        setInterval(() => {
            hand.style.transform = 'rotate(10deg) scale(1.1)';
            setTimeout(() => hand.style.transform = 'rotate(0deg) scale(1)', 200);
        }, 3000);
    }
</script>
<!-- custom slow spin for react logo -->
<style>
    .animate-spin-slow {
        animation: spin 10s linear infinite;
    }
    @keyframes spin {
        from { transform: rotate(0deg); }
        to { transform: rotate(360deg); }
    }
    /* glow enhancements */
    .card-shine {
        backdrop-filter: blur(2px);
    }
    h1 span {
        transition: transform 0.2s ease;
    }
</style>
</body>
</html>
