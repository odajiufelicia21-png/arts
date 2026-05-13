<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beat & Flow Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;700;900&display=swap');
body {
            font-family: 'Inter', sans-serif;
            background-color: #0a0a0c;
            color: white;
            scroll-behavior: smooth;
        }

        .custom-scrollbar::-webkit-scrollbar {
            width: 5px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.02);
            border-radius: 10px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: rgba(168, 85, 247, 0.3);
            border-radius: 10px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb:hover {
            background: rgba(168, 85, 247, 0.6);
        }

        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
.module-btn.active {
            background: linear-gradient(to right, #9333ea, #6b21a8);
            border-color: #c084fc;
            box-shadow: 0 10px 15px -3px rgba(88, 28, 135, 0.2);
        }
    </style>
</head>
<body class="pb-20">

    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 bg-[#0a0a0c]/80 backdrop-blur-md border-b border-white/10 px-6 py-4 flex justify-between items-center">
        <div class="flex items-center gap-2 cursor-pointer" onclick="switchTab('home')">
            <div class="w-10 h-10 bg-gradient-to-tr from-purple-600 to-cyan-400 rounded-lg flex items-center justify-center font-bold text-xl italic shadow-lg shadow-purple-500/20">B</div>
            <span class="text-xl font-black tracking-tighter uppercase hidden sm:inline">Beat & Flow <span class="text-purple-400 font-normal">Academy</span></span>
        </div>
        <div class="flex gap-4 md:gap-8 text-xs md:text-sm font-medium uppercase tracking-widest text-gray-400">
            <button onclick="switchTab('home')" id="nav-home" class="hover:text-purple-400 transition text-white border-b-2 border-purple-500 pb-1">Acasă</button>
            <button onclick="switchTab('curriculum')" id="nav-curriculum" class="hover:text-purple-400 transition">Curs</button>
            <button onclick="switchTab('pricing')" id="nav-pricing" class="hover:text-purple-400 transition">Preț</button>
        </div>
<button class="bg-purple-600 hover:bg-purple-500 px-4 md:px-6 py-2 rounded-full text-xs md:text-sm font-bold transition transform hover:scale-105 active:scale-95 shadow-lg shadow-purple-500/20">
            Acces Premium
        </button>
    </nav>

    <!-- SECTION: HOME -->
    <div id="home" class="tab-content active">
        <section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <div class="inline-flex items-center gap-2 px-3 py-1 bg-white/5 border border-white/10 rounded-full text-xs font-bold text-purple-400 mb-6 uppercase tracking-widest">
                        <i class="fas fa-bolt text-[10px]"></i> Revoluția Artistică Digitală
                    </div>
                    <h1 class="text-5xl md:text-8xl font-black leading-none mb-6 italic tracking-tighter uppercase">
                        MUZICA <span class="text-transparent bg-clip-text bg-gradient-to-r from-purple-400 to-cyan-400">ESTE</span> MIȘCARE.
                    </h1>
                    <p class="text-xl text-gray-400 mb-8 max-w-lg leading-relaxed font-light">
                        Singura platformă care te învață să produci propriul sunet și să-l transformi în mișcare scenică. Devino un artist complet 360°.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4">
<button onclick="switchTab('curriculum')" class="flex items-center justify-center gap-2 bg-white text-black px-8 py-4 rounded-xl font-bold text-lg hover:bg-gray-200 transition">
                            Explorează Modulele <i class="fas fa-arrow-right ml-2 text-sm"></i>
                        </button>
                    </div>
                </div>
                <div class="relative group">
                    <div class="absolute inset-0 bg-gradient-to-r from-purple-500/20 to-cyan-500/20 blur-3xl group-hover:from-purple-500/30 group-hover:to-cyan-500/30 transition"></div>
                    <div class="relative aspect-[4/5] rounded-3xl overflow-hidden border border-white/10 shadow-2xl">
                        <img src="https://images.unsplash.com/photo-1547153760-18fc86324498?q=80&w=1887&auto=format&fit=crop" alt="Coregrafie modernă" class="w-full h-full object-cover grayscale brightness-75 group-hover:grayscale-0 group-hover:brightness-100 transition duration-1000 scale-105 group-hover:scale-100">
                        <div class="absolute inset-0 bg-gradient-to-t from-[#0a0a0c] via-transparent to-transparent opacity-60"></div>
                        <div class="absolute bottom-8 left-8 right-8">
                            <div class="bg-black/60 backdrop-blur-xl p-6 rounded-2xl border border-white/10">
                                <div class="flex items-center gap-4 mb-3">
                                   <div class="w-2 h-2 bg-red-500 rounded-full animate-ping"></div>
                                   <span class="text-[10px] font-bold uppercase tracking-widest text-gray-300">Sesiune Live Acum</span>
                                </div>
<p class="font-bold italic text-lg leading-tight uppercase">Masterclass: Tehnici de Freestyle & Beat-making</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Gallery - 3 IMAGES -->
        <section class="px-6 max-w-7xl mx-auto py-20">
            <h2 class="text-sm font-bold uppercase tracking-[0.4em] text-center mb-12 text-gray-500">Vizualizarea Artei</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 h-[400px]">
                <div
class="rounded-2xl overflow-hidden border border-white/10 relative group shadow-2xl">
                    <img src="https://images.unsplash.com/photo-1516280440614-37939bbacd81?q=80&w=2070&auto=format&fit=crop" class="w-full h-full object-cover transition duration-500 group-hover:scale-110" alt="Concert">
                    <div class="absolute inset-0 bg-purple-600/20 opacity-0 group-hover:opacity-100 transition"></div>
                    <div class="absolute bottom-4 left-4 font-black italic uppercase text-xs tracking-widest">Performance</div>
https://images.unsplash.com/photo-1535525153412-5a42439a210d?q=80&w=2070&auto=format&fit=crop
 </div>
                <div class="rounded-2xl overflow-hidden border border-white/10 relative group shadow-2xl">
                    <img src="https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?q=80&w=2070&auto=format&fit=crop" class="w-full h-full object-cover transition duration-500 group-hover:scale-110" alt="Studio">
                    <div class="absolute inset-0 bg-purple-600/20 opacity-0 group-hover:opacity-100 transition"></div>
                    <div class="absolute bottom-4 left-4 font-black italic uppercase text-xs tracking-widest">Production</div>
 </div>
            </div>
        </section>
    </div>

    <!-- SECTION: CURRICULUM -->
    <div id="curriculum" class="tab-content">
        <section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-end mb-16 gap-6">
                <div>
                    <h2 class="text-4xl md:text-6xl font-black italic mb-2 uppercase tracking-tighter">Plan de <span class="text-purple-400">Carieră</span></h2>
                    <p
class="text-gray-400 text-lg">10 pași spre măiestria artistică totală.</p>
                </div>
                <div class="flex gap-4 bg-white/5 p-2 rounded-2xl border border-white/10">
                   <div class="px-4 py-2 bg-purple-600 rounded-xl font-bold text-xs uppercase tracking-widest">Studenți: 12.4k</div>
                   <div class="px-4 py-2 border border-white/10 rounded-xl font-bold text-xs uppercase tracking-widest">Update: 2026</div>
                </div>
            </div>
<div class="grid lg:grid-cols-12 gap-10">
                <!-- Sidebar -->
                <div id="module-list" class="lg:col-span-4 space-y-3 h-[700px] overflow-y-auto pr-4 custom-scrollbar">
                    <!-- Modules will be injected here -->
                </div>

                <!-- Module Detail -->
                <div class="lg:col-span-8">
                    <div class="bg-white/5 rounded-[2.5rem] border border-white/10 overflow-hidden shadow-2xl" id="module-display">
                        <!--
Module content injected here -->
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- SECTION: PRICING -->
    <div id="pricing" class="tab-content">
        <section class="pt-32 pb-20 px-6 max-w-7xl mx-auto text-center">
            <h2 class="text-5xl md:text-7xl font-black italic mb-4 uppercase tracking-tighter">Investiția în <span class="text-purple-400">Arta</span> Ta</h2>
            <p class="text-gray-400 max-w-2xl mx-auto text-lg mb-16 font-light leading-relaxed">
                Pachete
create pentru orice nivel de experiență. De la explorator curios la artist de scenă.
            </p>

            <div class="grid md:grid-cols-3 gap-8 items-center">
                <!-- Explorer -->
                <div class="bg-gray-800 p-10 rounded-[2.5rem] border border-white/10 flex flex-col items-center text-left relative overflow-hidden group hover:shadow-2xl hover:shadow-purple-500/20 transition-all duration-500">
                    <h3 class="text-2xl font-black italic uppercase mb-2">Explorer</h3>
                    <div
class="text-5xl font-black mb-8 italic tracking-tighter">49€ <span class="text-sm font-normal text-gray-500 uppercase tracking-widest">/ total</span></div>
                    <div class="w-full h-px bg-white/10 mb-8"></div>
                    <ul class="space-y-4 mb-10 w-full text-sm text-gray-300 font-medium">
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Modulele 1-4</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Acces 6 luni</li>
                        <li
class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Glosar Termeni</li>
                    </ul>
                    <button class="w-full py-5 rounded-2xl font-black uppercase tracking-[0.2em] text-xs bg-white/5 text-white hover:bg-white/10 transition-all">Cumpără Acum</button>
                </div>
                <!-- PRO -->
                <div class="bg-purple-900 border-2 border-purple-400 scale-105 p-10 rounded-[2.5rem] flex flex-col items-center text-left relative overflow-hidden group hover:shadow-2xl hover:shadow-purple-500/20 transition-all duration-500">
                    <div
class="absolute top-6 right-6 bg-cyan-400 text-black px-3 py-1 rounded-full text-[10px] font-black uppercase italic animate-pulse">Cel Mai Popular</div>
                    <h3 class="text-2xl font-black italic uppercase mb-2">Artist PRO</h3>
                    <div class="text-5xl font-black mb-8 italic tracking-tighter">129€ <span class="text-sm font-normal text-gray-500/50 uppercase tracking-widest">/ total</span></div>
                    <div class="w-full h-px bg-white/10 mb-8"></div>
                    <ul class="space-y-4 mb-10 w-full text-sm text-gray-300 font-medium">
                        <li
class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Toate cele 10 Module</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Plan de 30/90 zile</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Acces Comunitate</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Checklist-uri</li>
                    </ul>
                    <button
class="w-full py-5 rounded-2xl font-black uppercase tracking-[0.2em] text-xs bg-white text-black hover:bg-purple-500 hover:text-white transition-all shadow-xl shadow-white/5">Cumpără Acum</button>
                </div>
                <!-- Elite -->
                <div class="bg-gray-900 p-10 rounded-[2.5rem] border border-white/10 flex flex-col items-center text-left relative overflow-hidden group hover:shadow-2xl hover:shadow-purple-500/20 transition-all duration-500">
                    <h3 class="text-2xl font-black italic uppercase mb-2">Elite Masterclass</h3>
                    <div
class="text-5xl font-black mb-8 italic tracking-tighter">299€ <span class="text-sm font-normal text-gray-500 uppercase tracking-widest">/ total</span></div>
                    <div class="w-full h-px bg-white/10 mb-8"></div>
                    <ul class="space-y-4 mb-10 w-full text-sm text-gray-300 font-medium">
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Tot din PRO</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Feedback Personalizat</li>
                        <li
class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> 1-on-1 Mentoring</li>
                        <li class="flex items-center gap-3"><i class="fas fa-check-circle text-purple-400"></i> Certificat de Absolvire</li>
                    </ul>
                    <button class="w-full py-5 rounded-2xl font-black uppercase tracking-[0.2em] text-xs bg-white/5 text-white hover:bg-white/10 transition-all">Cumpără Acum</button>
                </div>
            </div>
        </section>
    </div>

    <!-- Stats -->
<section class="bg-white/5 py-20 border-y border-white/10 px-6 mt-10">
        <div class="max-w-7xl mx-auto grid grid-cols-2 md:grid-cols-4 gap-12 text-center">
            <div>
                <span class="block text-4xl md:text-5xl font-black italic text-purple-400 mb-2 uppercase tracking-tighter">150+</span>
                <span class="text-xs font-bold uppercase tracking-widest text-gray-500">Video Lecții</span>
            </div>
            <div>
                <span class="block text-4xl md:text-5xl font-black italic text-white mb-2 uppercase tracking-tighter">45GB</span>
                <span
class="text-xs font-bold uppercase tracking-widest text-gray-500">Resurse Audio</span>
            </div>
            <div>
                <span class="block text-4xl md:text-5xl font-black italic text-cyan-400 mb-2 uppercase tracking-tighter">24/7</span>
                <span class="text-xs font-bold uppercase tracking-widest text-gray-500">Suport Comunitate</span>
            </div>
            <div>
                <span class="block text-4xl md:text-5xl font-black italic text-white mb-2 uppercase tracking-tighter">LIFETIME</span>
<span class="text-xs font-bold uppercase tracking-widest text-gray-500">Acces Conținut</span>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="mt-20 border-t border-white/10 py-16 px-6 bg-black">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-4 gap-12 mb-16">
                <div class="col-span-2">
                   <div class="flex items-center gap-2 mb-6">
                    <div class="w-10 h-10
bg-purple-600 rounded flex items-center justify-center font-bold italic shadow-lg shadow-purple-500/20">B</div>
                    <span class="text-xl font-black italic uppercase tracking-tighter">Beat & Flow <span class="text-purple-400">Academy</span></span>
                  </div>
                  <p class="text-gray-500 max-w-sm leading-relaxed italic">Transformăm pasiunea în profesie. O metodologie unică ce unește sunetul cu mișcare corporală.</p>
                </div>
                <div>
                  <h5 class="font-bold uppercase tracking-widest text-xs mb-6 text-white">Comunitate</h5>
                  <ul class="space-y-4 text-sm
text-gray-500 font-medium">
                    <li class="hover:text-purple-400 cursor-pointer transition">Grup de Discord</li>
                    <li class="hover:text-purple-400 cursor-pointer transition">Evenimente Live</li>
                    <li class="hover:text-purple-400 cursor-pointer transition">Showcase-ul Elevilor</li>
                  </ul>
                </div>
                <div>
                  <h5 class="font-bold uppercase tracking-widest text-xs mb-6 text-white">Legal</h5>
                  <ul class="space-y-4 text-sm text-gray-500 font-medium">
                    <li
class="hover:text-purple-400 cursor-pointer transition">Termeni și Condiții</li>
                    <li class="hover:text-purple-400 cursor-pointer transition">Politică de Confidențialitate</li>
                    <li class="hover:text-purple-400 cursor-pointer transition">Contact Media</li>
                  </ul>
                </div>
            </div>
            <div class="pt-8 border-t border-white/5 flex flex-col md:flex-row justify-between items-center gap-8">
                <p class="text-gray-600 text-[10px] uppercase tracking-[0.3em] font-bold italic">© 2026 Beat & Flow Academy — Premium Arts Education</p>
<div class="flex gap-8">
                  <i class="fas fa-mobile-alt text-gray-600 hover:text-white cursor-pointer transition-colors"></i>
                  <i class="fas fa-broadcast-tower text-gray-600 hover:text-white cursor-pointer transition-colors"></i>
                  <i class="fas fa-layer-group text-gray-600 hover:text-white cursor-pointer transition-colors"></i>
                </div>
            </div>
        </div>
    </footer>

    <script>
        const modulesData = [
            { id: 1, title: "M1: Introducere în Simbioza Artistică",
subtitle: "Creierul, Ritmul și Mișcarea", image: "https://images.unsplash.com/photo-1514525253361-bee8a18744ad?q=80&w=1964&auto=format&fit=crop", content: "Descoperă cum reacționează creierul la frecvențe și cum se transformă sunetul în impuls muscular. Explicația științifică a legăturii dintre sunet și mișcare.", exercises: ["Ascultare activă: Identificarea instrumentelor", "Coordonare 4/4 cu palmele", "Jurnal de expresie emoțională"], lessons: ["Ce este muzica?", "Evoluția dansului", "Neuroștiința ritmului", "Legătura sunet-corp"] },
            { id: 2, title: "M2: Arhitectura Muzicală", subtitle: "De la Notă la
Emoție", image: "https://images.unsplash.com/photo-1507838153414-b4b713384a76?q=80&w=2070&auto=format&fit=crop", content: "Învață alfabetul muzical: note, game, acorduri, tempo și structuri compoziționale moderne. Diferența dintre genuri și BPM.", lessons: ["Note și Gamă", "BPM și Ritm", "Armonie și Emoție", "Structura unei piese Pop/EDM"] },
            { id: 3, title: "M3: Templul Mișcării", subtitle: "Postură, Echilibru și Control", image: "https://images.unsplash.com/photo-1508700115892-45ecd05ae2ad?q=80&w=2069&auto=format&fit=crop", content: "Pregătirea fizică a artistului. Tehnici de stretching, izolare corporală și prevenirea accidentărilor pentru o carieră lungă.", lessons: ["Postura Corectă", "Centre de Echilibru", "Mobilitate
Articulară", "Izolări: Gât, Umeri, Șolduri"] },
            { id: 4, title: "M4: Enciclopedia Stilurilor", subtitle: "Genuri Muzicale & Dansuri Urbane", image: "https://images.unsplash.com/photo-1535525153412-5a42439a210d?q=80&w=2070&auto=format&fit=crop", content: "O incursiune în Hip-Hop, Contemporary, K-Pop, Salsa și Afrobeat. Istorie, ritm specific și artiști celebri.", lessons: ["Hip-Hop Culture", "Contemporary Flow", "K-Pop Industry", "Afrobeat Rhythms"] },
            { id: 5, title: "M5: Laboratorul de Producție", subtitle: "Crearea Primului Tău Beat", image: "https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?q=80&w=2070&auto=format&fit=crop", content: "Introducere în DAW-uri: FL Studio, Ableton, Logic. Beat
making, sample-uri, mixaj și efecte audio de bază.", lessons: ["Alegerea DAW-ului", "Sound Design & Sample-uri", "Mixajul Vocilor", "Efecte: Reverb, Delay"] },
            { id: 6, title: "M6: Arta Coregrafică", subtitle: "Vizualizarea Muzicii", image: "https://images.unsplash.com/photo-1547153760-18fc86324498?q=80&w=1887&auto=format&fit=crop", content: "Cum să construiești o poveste prin mișcare. Sincronizare pe beat, tranziții fluide și energie scenică impunătoare.", lessons: ["Conceptul Coregrafic", "Tranziții Fluide", "Sincronizarea pe Beat", "Freestyle"] },
            { id: 7, title: "M7: Business & Branding", subtitle: "Industria Muzicală
Modernă", image: "https://images.unsplash.com/photo-1559136555-9303baea8ebd?q=80&w=2070&auto=format&fit=crop", content: "Navigarea pe platformele Spotify, YouTube și Instagram. Cum devii un artist independent și cum îți lansezi muzica.", lessons: ["Distribuție Digitală", "Branding de Artist", "Monetizare", "Networking"] },
            { id: 8, title: "M8: Viralitate pe Social Media", subtitle: "Strategii TikTok & Instagram", image: "https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?q=80&w=1974&auto=format&fit=crop", content: "Crearea de conținut care atrage atenția. Algoritmi, estetică vizuală și storytelling artistic pentru reels și shorts.", lessons: ["Algoritmul TikTok", "Estetică Visuală", "Strategii de Reels", "Comunitatea de
Fani"] },
            { id: 9, title: "M9: Psihologia Scenică", subtitle: "Mentalitate de Învingător", image: "https://images.unsplash.com/photo-1516280440614-37939bbacd81?q=80&w=2070&auto=format&fit=crop", content: "Emoția ca instrument de lucru. Depășirea fricii de scenă, disciplina creativă și menținerea încrederii în viziunea ta.", lessons: ["Încrederea pe Scenă", "Depășirea Blocajelor", "Disciplina", "Emoția ca Instrument"] },
            { id: 10, title: "M10: Marea Lansare", subtitle: "De la Dormitor la Scenă", image: "https://images.unsplash.com/photo-1470225620780-dba8ba36b745?q=80&w=2070&auto=format&fit=crop", content: "Ghid complet de lansare a primei
melodii și a primului videoclip. Plan de promovare și analiză a rezultatelor.", lessons: ["Planul de Lansare", "Producția Video", "Campania de PR", "Analiza Rezultatelor"] }
        ];

        let activeModuleIndex = 0;

        function switchTab(tabId) {
            document.querySelectorAll('.tab-content').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
            
            // Update Nav Styles
document.querySelectorAll('nav button').forEach(btn => {
                btn.classList.remove('text-white', 'border-b-2', 'border-purple-500', 'pb-1');
            });
            document.getElementById('nav-' + tabId).classList.add('text-white', 'border-b-2', 'border-purple-500', 'pb-1');

            if(tabId === 'curriculum') {
                renderModuleList();
                renderModuleDetail(activeModuleIndex);
            }
        }

        function renderModuleList() {
            const list = document.getElementById('module-list');
list.innerHTML = modulesData.map((m, idx) => `
                <button onclick="setActiveModule(${idx})" class="module-btn w-full text-left p-6 rounded-2xl transition-all duration-300 border group ${activeModuleIndex === idx ? 'module-btn active' : 'bg-white/5 border-white/10 hover:bg-white/10 hover:border-white/20'}">
                    <div class="flex justify-between items-start mb-2">
                        <span class="text-[10px] font-black uppercase tracking-[0.2em] ${activeModuleIndex === idx ? 'text-white/70' : 'text-purple-400'}">Modulul 0${m.id}</span>
                        ${activeModuleIndex === idx ? '<i class="fas fa-play text-[8px]"></i>' : ''}
</div>
                    <span class="text-lg font-black italic uppercase leading-none block group-hover:translate-x-1 transition-transform">${m.title.split(': ')[1]}</span>
                </button>
            `).join('');
        }

        function setActiveModule(index) {
            activeModuleIndex = index;
            renderModuleList();
            renderModuleDetail(index);
        }

        function renderModuleDetail(idx) {
            const m = modulesData[idx];
const display = document.getElementById('module-display');
            
            display.innerHTML = `
                <div class="h-64 w-full relative">
                    <img src="${m.image}" class="w-full h-full object-cover" alt="Module Image">
                    <div class="absolute inset-0 bg-gradient-to-t from-[#121214] via-black/20 to-transparent"></div>
                    <div class="absolute bottom-6 left-8">
                        <h3 class="text-3xl font-black italic uppercase tracking-tighter text-white drop-shadow-lg">${m.title}</h3>
                        <p
class="text-purple-400 font-bold uppercase text-xs tracking-widest">${m.subtitle}</p>
                    </div>
                </div>
                <div class="p-8 md:p-12">
                    <div class="grid md:grid-cols-3 gap-12">
                        <div class="md:col-span-2">
                            <h4 class="text-xs font-bold text-gray-500 uppercase tracking-[0.3em] mb-6">Obiective de învățare</h4>
                            <p class="text-xl text-gray-300 leading-relaxed italic mb-10">"${m.content}"</p>
                            <div class="grid sm:grid-cols-2 gap-8">
<div>
                                    <h5 class="text-[10px] font-bold text-white uppercase tracking-widest mb-4 flex items-center gap-2">
                                        <i class="fas fa-layer-group text-cyan-400"></i> Programa Detaliată
                                    </h5>
                                    <ul class="space-y-4">
                                        ${m.lessons.map(l => `
                                            <li class="flex items-center gap-3 text-sm text-gray-400">
                                                <div class="w-1 h-1 bg-purple-500 rounded-full"></div>
                                                ${l}
                                            </li>

`).join('')}
                                    </ul>
                                </div>
                                ${m.exercises ? `
                                    <div class="bg-purple-900/10 p-6 rounded-2xl border border-purple-500/20">
                                        <h5 class="text-[10px] font-bold text-purple-400 uppercase tracking-widest mb-4 flex items-center gap-2">
                                            <i class="fas fa-bolt text-xs"></i> Workshop Practic
                                        </h5>
                                        <ul class="space-y-3">
                                            ${m.exercises.map(ex => `
                                                <li class="text-xs font-medium text-gray-300
italic border-l-2 border-purple-500/40 pl-3">
                                                    ${ex}
                                                </li>
                                            `).join('')}
                                        </ul>
                                    </div>
                                ` : ''}
                            </div>
                        </div>
                        <div class="space-y-6">
                            <div class="bg-black/40 p-6 rounded-2xl border border-white/5">
                                <h4 class="text-[10px] font-bold uppercase
text-gray-500 mb-4 tracking-widest">Resurse Modul</h4>
                                <div class="space-y-3">
                                    <button class="w-full flex items-center gap-3 p-3 rounded-lg bg-white/5 hover:bg-white/10 transition text-xs font-bold uppercase tracking-widest text-left">
                                        <i class="fas fa-file-pdf text-purple-400"></i> Ghid PDF
                                    </button>
                                    <button class="w-full flex items-center gap-3 p-3 rounded-lg bg-white/5 hover:bg-white/10 transition text-xs font-bold uppercase tracking-widest text-left">
                                        <i class="fas fa-music text-cyan-400"></i> Playlist
</button>
                                    <button class="w-full flex items-center gap-3 p-3 rounded-lg bg-white/5 hover:bg-white/10 transition text-xs font-bold uppercase tracking-widest text-left">
                                        <i class="fas fa-video"></i> Live Replay
                                    </button>
                                </div>
                            </div>
                            <div class="p-6 bg-gradient-to-br from-purple-600/20 to-transparent rounded-2xl border border-purple-500/20">
                                <i class="fas fa-chart-line
text-purple-400 text-2xl mb-4 block"></i>
                                <p class="text-xs text-gray-400 font-medium">Acest modul îți va crește coordonarea cu <span class="text-white font-bold">40%</span> în prima săptămână.</p>
                            </div>
                        </div>
                    </div>
                    <div class="mt-12 pt-10 border-t border-white/5 flex flex-col sm:flex-row justify-between items-center gap-6">
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-full border border-white/10 overflow-hidden">
<img src="https://images.unsplash.com/photo-1539571696357-5a69c17a67c6?q=80&w=1887&auto=format&fit=crop" class="w-full h-full object-cover" alt="Expert">
                            </div>
                            <div>
                                <span class="block text-xs font-bold uppercase tracking-widest text-purple-400">Expert Instructor</span>
                                <span class="text-sm font-black italic uppercase">Alex Voinea</span>
                            </div>
                        </div>
                        <button class="bg-white text-black px-10 py-4
rounded-xl font-black uppercase tracking-[0.2em] text-sm hover:bg-purple-500 hover:text-white transition transform active:scale-95 flex items-center gap-3 shadow-xl">
                            Începe Învățarea <i class="fas fa-play text-xs"></i>
                        </button>
                    </div>
                </div>
            `;
        }
    </script>
</body>
