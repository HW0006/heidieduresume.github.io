# heidieduresume.github.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- SEO & Professional Metadata -->
    <title>Han Yu Wang | Student Counselor & Education Strategist</title>
    <meta name="description" content="Bilingual Student Counselor specializing in study planning, parent consulting, and operational excellence for EdTech and coding programs.">
    <meta property="og:title" content="Han Yu Wang | Student Counselor Profile">
    <meta property="og:description" content="Leveraging clinical empathy and logistical precision to guide the next generation of tech leaders.">
    <meta property="og:type" content="website">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Three.js for 3D Earth -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: transparent; 
            color: #0f172a; 
            overflow-x: hidden;
        }

        #bg-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: -1;
            background: radial-gradient(circle at center, #ffffff 0%, #f0f4f8 100%);
        }

        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
            background: rgba(255, 255, 255, 0.5);
            backdrop-filter: blur(12px);
            border-radius: 32px;
            padding: 24px;
        }
        
        @media (min-width: 768px) {
            .chart-container { height: 360px; }
        }

        .edu-card {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.5);
            border-radius: 32px;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.02);
            transition: all 0.5s cubic-bezier(0.16, 1, 0.3, 1);
            position: relative;
            overflow: hidden;
        }

        .edu-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 25px 50px -12px rgba(79, 70, 229, 0.1);
            border-color: rgba(79, 70, 229, 0.3);
        }

        .nav-link {
            position: relative;
            font-weight: 700;
            transition: all 0.3s ease;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 3px;
            bottom: -6px;
            left: 50%;
            background: #4f46e5;
            transition: all 0.3s ease;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        .nav-link:hover::after { width: 24px; }

        .filter-btn {
            border-radius: 16px;
            transition: all 0.3s ease;
            border: 1px solid rgba(0,0,0,0.05);
            background: white;
            font-weight: 700;
            font-size: 0.75rem;
            letter-spacing: 0.05em;
        }

        .filter-btn.active {
            background-color: #4f46e5;
            color: white;
            border-color: #4f46e5;
            box-shadow: 0 10px 20px -5px rgba(79, 70, 229, 0.4);
        }

        .glass-tag {
            background: rgba(79, 70, 229, 0.1);
            color: #4f46e5;
            padding: 4px 12px;
            border-radius: 10px;
            font-weight: 700;
            font-size: 10px;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <canvas id="bg-canvas"></canvas>

    <nav class="bg-white/50 backdrop-blur-2xl border-b border-white/50 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20">
                <div class="flex items-center">
                    <span class="text-xl font-extrabold text-slate-900 tracking-tighter flex items-center">
                        <i class="fa-solid fa-star mr-2 text-indigo-600 animate-pulse"></i> HAN YU WANG
                    </span>
                </div>
                <div class="hidden md:flex items-center space-x-10 text-[11px] uppercase tracking-widest font-extrabold">
                    <a href="#summary" class="nav-link text-slate-500 hover:text-indigo-600">The Mission</a>
                    <a href="#competencies" class="nav-link text-slate-500 hover:text-indigo-600">Mastery</a>
                    <a href="#experience" class="nav-link text-slate-500 hover:text-indigo-600">Worklogs</a>
                    <a href="#credentials" class="nav-link text-slate-500 hover:text-indigo-600">Credentials</a>
                </div>
            </div>
        </div>
    </nav>

    <main class="flex-grow">
        <!-- Hero Section -->
        <section id="summary" class="py-24">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
                    <div class="fade-in">
                        <div class="inline-flex items-center px-4 py-2 bg-indigo-50 text-indigo-600 text-[10px] font-extrabold uppercase mb-8 rounded-2xl border border-indigo-100 shadow-sm">
                            <span class="w-2 h-2 rounded-full bg-indigo-500 mr-2"></span>
                            Target Role: X-Camp Student Counselor
                        </div>
                        <h1 class="text-5xl md:text-7xl font-extrabold text-slate-900 mb-8 tracking-tighter leading-none">
                            Guiding the <br/><span class="text-indigo-600">Future of Code.</span>
                        </h1>
                        <p class="text-lg text-slate-600 mb-10 leading-relaxed max-w-xl font-medium">
                            Synthesizing <span class="text-slate-900 font-bold">Clinical Empathy</span> with <span class="text-slate-900 font-bold">Operational Data</span>. 
                            Bilingual professional dedicated to optimizing student success and parent partnerships in the Bay Area EdTech ecosystem.
                        </p>
                        <div class="flex flex-wrap gap-4 text-slate-500 text-[12px] font-bold">
                            <div class="flex items-center px-5 py-3 bg-white/90 rounded-2xl shadow-sm border border-white/50 backdrop-blur-md">
                                <i class="fa-solid fa-map-pin mr-3 text-indigo-600"></i> BAY AREA, CA
                            </div>
                            <div class="flex items-center px-5 py-3 bg-white/90 rounded-2xl shadow-sm border border-white/50 backdrop-blur-md">
                                <i class="fa-solid fa-envelope mr-3 text-indigo-600"></i> heidiwangprofessional@gmail.com
                            </div>
                            <div class="flex items-center px-5 py-3 bg-white/90 rounded-2xl shadow-sm border border-white/50 backdrop-blur-md">
                                <i class="fa-solid fa-phone mr-3 text-indigo-600"></i> 408-455-0322
                            </div>
                        </div>
                    </div>
                    
                    <div class="relative">
                        <div class="relative bg-white/70 backdrop-blur-3xl p-10 rounded-[48px] shadow-2xl border border-white">
                            <h3 class="text-[10px] font-bold text-slate-400 mb-8 tracking-[0.2em] uppercase">Core_Counseling_Metrics</h3>
                            <div class="space-y-6">
                                <div class="flex items-center">
                                    <div class="w-12 h-12 rounded-2xl bg-indigo-600 text-white flex items-center justify-center mr-5 shadow-lg">
                                        <i class="fa-solid fa-language"></i>
                                    </div>
                                    <div>
                                        <span class="block font-extrabold text-slate-900">Bilingual: Mandarin & English</span>
                                        <span class="text-[10px] text-slate-400 uppercase font-bold">Native-Level Communication</span>
                                    </div>
                                </div>
                                <div class="flex items-center">
                                    <div class="w-12 h-12 rounded-2xl bg-indigo-600 text-white flex items-center justify-center mr-5 shadow-lg">
                                        <i class="fa-solid fa-chart-pie"></i>
                                    </div>
                                    <div>
                                        <span class="block font-extrabold text-slate-900">Data-Driven Consulting</span>
                                        <span class="text-[10px] text-slate-400 uppercase font-bold">Student Progress Tracking</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Mastery Section -->
        <section id="competencies" class="py-24 bg-white/20">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="mb-20 text-center">
                    <h2 class="text-3xl font-extrabold text-slate-900 mb-6 tracking-tight">Student Success & Operational Strategy</h2>
                    <p class="text-slate-500 max-w-xl mx-auto font-medium">Alignment analysis based on X-Camp's Counselor requirements.</p>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                    <div class="edu-card p-10">
                        <h3 class="text-[11px] font-extrabold text-slate-400 uppercase mb-10">Skill Alignment Radar</h3>
                        <div class="chart-container">
                            <canvas id="competencyRadarChart"></canvas>
                        </div>
                    </div>
                    <div class="edu-card p-10">
                        <h3 class="text-[11px] font-extrabold text-slate-400 uppercase mb-10">Functional Strengths</h3>
                        <div class="chart-container">
                            <canvas id="skillsBarChart"></canvas>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Worklogs Section -->
        <section id="experience" class="py-24">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex flex-col md:flex-row md:items-center justify-between mb-16 gap-8">
                    <h2 class="text-3xl font-extrabold text-slate-900 tracking-tight">Mission Chronicles: Career Logs</h2>
                    <div class="flex flex-wrap gap-2" id="experience-filters">
                        <button onclick="filterExperience('all')" class="filter-btn active px-6 py-2.5">ALL_RECORDS</button>
                        <button onclick="filterExperience('consulting')" class="filter-btn px-6 py-2.5">COUNSELING</button>
                        <button onclick="filterExperience('operations')" class="filter-btn px-6 py-2.5">OPS & DATA</button>
                    </div>
                </div>
                <div id="experience-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10"></div>
            </div>
        </section>
    </main>

    <footer class="bg-white/30 backdrop-blur-xl border-t border-slate-100 py-16 mt-auto">
        <div class="max-w-7xl mx-auto px-4 text-center">
            <div class="text-[10px] tracking-[0.5em] mb-10 text-slate-300 font-extrabold uppercase">Mission Control: Global Education</div>
            <p class="text-[10px] font-extrabold text-slate-400 tracking-widest uppercase">&copy; 2025 HAN YU WANG // PORTFOLIO FOR X-CAMP</p>
        </div>
    </footer>

    <script>
        // --- THREE.JS EARTH ---
        let scene, camera, renderer, globe, particles;
        let mouseX = 0, mouseY = 0;

        function initThree() {
            const canvas = document.getElementById('bg-canvas');
            scene = new THREE.Scene();
            camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
            renderer = new THREE.WebGLRenderer({ canvas, antialias: true, alpha: true });
            renderer.setSize(window.innerWidth, window.innerHeight);
            renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));

            const geometry = new THREE.SphereGeometry(4, 64, 64);
            const material = new THREE.MeshBasicMaterial({ color: 0x4f46e5, wireframe: true, transparent: true, opacity: 0.04 });
            globe = new THREE.Mesh(geometry, material);
            scene.add(globe);

            const pGeometry = new THREE.BufferGeometry();
            const pCount = 2000;
            const posArray = new Float32Array(pCount * 3);
            for(let i=0; i < pCount * 3; i++) { posArray[i] = (Math.random() - 0.5) * 25; }
            pGeometry.setAttribute('position', new THREE.BufferAttribute(posArray, 3));
            particles = new THREE.Points(pGeometry, new THREE.PointsMaterial({ size: 0.012, color: 0x4f46e5, transparent: true, opacity: 0.2 }));
            scene.add(particles);

            camera.position.z = 10;
            window.addEventListener('resize', () => {
                camera.aspect = window.innerWidth / window.innerHeight;
                camera.updateProjectionMatrix();
                renderer.setSize(window.innerWidth, window.innerHeight);
            });
            document.addEventListener('mousemove', (e) => {
                mouseX = (e.clientX - window.innerWidth / 2) * 0.0006;
                mouseY = (e.clientY - window.innerHeight / 2) * 0.0006;
            });
            animate();
        }

        function animate() {
            requestAnimationFrame(animate);
            globe.rotation.y += 0.002 + (mouseX * 0.1);
            globe.rotation.x += (mouseY * 0.1);
            particles.rotation.y -= 0.0005;
            renderer.render(scene, camera);
        }

        // --- DATA ---
        const experienceData = [
            { id: 1, role: "Bilingual Family Consultant", company: "Camino Pediatric", date: "2025", type: ["consulting", "operations"], description: "Bridge English-Mandarin comms for pediatric services. Managed detailed patient documentation and parent expectations.", icon: "fa-users" },
            { id: 2, role: "Operational Logistics Manager", company: "Belmont Village", date: "2024-25", type: ["operations"], description: "Directed daily operations and multicultural coordination. Expert in scheduling and high-pressure logistical oversight.", icon: "fa-layer-group" },
            { id: 3, role: "Public Health Liaison", company: "Health Center (Taiwan)", date: "2024", type: ["consulting"], description: "Bilingual student and family outreach. Managed medical record data and educational deliverable creation.", icon: "fa-comments" }
        ];

        function renderExperience(filter = 'all') {
            const grid = document.getElementById('experience-grid');
            grid.innerHTML = '';
            const filteredData = filter === 'all' ? experienceData : experienceData.filter(item => item.type.includes(filter));
            filteredData.forEach(job => {
                const card = document.createElement('div');
                card.className = "edu-card p-10 flex flex-col h-full";
                card.innerHTML = `
                    <div class="flex justify-between items-start mb-8">
                        <div class="w-12 h-12 rounded-2xl bg-indigo-600 text-white flex items-center justify-center text-xl shadow-lg"><i class="fa-solid ${job.icon}"></i></div>
                        <span class="text-[9px] font-extrabold text-slate-300 bg-slate-50 px-3 py-1 rounded-full uppercase tracking-widest">${job.date}</span>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-2">${job.role}</h3>
                    <p class="text-[10px] font-bold text-slate-400 mb-6 uppercase tracking-widest">${job.company}</p>
                    <p class="text-sm text-slate-500 mb-8 flex-grow leading-relaxed font-medium">${job.description}</p>
                    <div class="flex flex-wrap gap-2 pt-6 border-t border-slate-100">${job.type.map(t => `<span class="glass-tag uppercase">${t}</span>`).join('')}</div>
                `;
                grid.appendChild(card);
            });
        }

        function filterExperience(type) {
            document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
            const activeBtn = Array.from(document.querySelectorAll('.filter-btn')).find(b => b.getAttribute('onclick').includes(type));
            if(activeBtn) activeBtn.classList.add('active');
            renderExperience(type);
        }

        function initCharts() {
            const ctxRadar = document.getElementById('competencyRadarChart').getContext('2d');
            new Chart(ctxRadar, {
                type: 'radar',
                data: {
                    labels: ['Bilingual Comms', 'Parent Consulting', 'Operational Tech', 'Data Tracking', 'Empathy/Support', 'Workflow Opt.'],
                    datasets: [{ label: 'Fit Alignment', data: [100, 95, 85, 90, 95, 88], backgroundColor: 'rgba(79, 70, 229, 0.1)', borderColor: '#4f46e5', borderWidth: 2 }]
                },
                options: { responsive: true, maintainAspectRatio: false, scales: { r: { suggestedMin: 0, suggestedMax: 100, ticks: { display: false }, pointLabels: { font: { family: 'Plus Jakarta Sans', size: 9, weight: '700' }, color: '#94a3b8' } } }, plugins: { legend: { display: false } } }
            });

            const ctxBar = document.getElementById('skillsBarChart').getContext('2d');
            new Chart(ctxBar, {
                type: 'bar',
                data: {
                    labels: ['Consulting', 'Mandarin', 'Operations', 'Data', 'Customer Exp'],
                    datasets: [{ data: [90, 100, 85, 80, 95], backgroundColor: ['#4f46e5', '#4338ca', '#3730a3', '#312e81', '#1e1b4b'], borderRadius: 10 }]
                },
                options: { responsive: true, maintainAspectRatio: false, scales: { y: { display: false }, x: { grid: { display: false }, ticks: { font: { family: 'Plus Jakarta Sans', size: 9, weight: '700' }, color: '#94a3b8' } } }, plugins: { legend: { display: false } } }
            });
        }

        window.onload = function() {
            initThree();
            renderExperience('all');
            initCharts();
        };
    </script>
</body>
</html>
