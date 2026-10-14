<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auwalun Nisa’ — Portofolio Soft Pastel & Creative PTI UNESA</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Poppins -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Poppins', 'sans-serif'],
                    },
                    colors: {
                        sage: '#76A08A',
                        sageLight: '#E8F0EC',
                        cream: '#F9F8F6',
                        peach: '#E8A598',
                        peachLight: '#FDF3F1',
                        lavender: '#9B8EC4',
                        lavenderLight: '#F2EFF7',
                        slateText: '#2F3E46',
                    }
                }
            }
        }
    </script>
    
    <style>
        body {
            background-color: #F9F8F6;
            color: #2F3E46;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
        }

        .pastel-card {
            background: #FFFFFF;
            border: 1px solid rgba(118, 160, 138, 0.15);
            box-shadow: 0 15px 35px rgba(47, 62, 70, 0.05);
            transition: all 0.3s ease;
        }

        .pastel-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 40px rgba(118, 160, 138, 0.12);
        }

        .pastel-nav {
            background: rgba(249, 248, 246, 0.85);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(118, 160, 138, 0.2);
        }

        .text-gradient {
            background: linear-gradient(135deg, #76A08A 0%, #9B8EC4 50%, #E8A598 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Decorative Pastel Blobs */
        .blob-bg-1 {
            position: absolute;
            top: 5%;
            left: 5%;
            width: 380px;
            height: 380px;
            background: rgba(118, 160, 138, 0.12);
            filter: blur(80px);
            border-radius: 50%;
            z-index: -1;
            pointer-events: none;
        }

        .blob-bg-2 {
            position: absolute;
            top: 35%;
            right: 5%;
            width: 420px;
            height: 420px;
            background: rgba(155, 142, 196, 0.1);
            filter: blur(90px);
            border-radius: 50%;
            z-index: -1;
            pointer-events: none;
        }

        .blob-bg-3 {
            position: absolute;
            bottom: 10%;
            left: 15%;
            width: 400px;
            height: 400px;
            background: rgba(232, 165, 152, 0.12);
            filter: blur(90px);
            border-radius: 50%;
            z-index: -1;
            pointer-events: none;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }
        ::-webkit-scrollbar-track {
            background: #F9F8F6;
        }
        ::-webkit-scrollbar-thumb {
            background: #76A08A;
            border-radius: 9999px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #5b7e6c;
        }
    </style>
</head>
<body class="antialiased selection:bg-sage selection:text-white relative">

    <div class="blob-bg-1"></div>
    <div class="blob-bg-2"></div>
    <div class="blob-bg-3"></div>

    <header class="fixed top-4 left-4 right-4 z-50 max-w-6xl mx-auto">
        <nav class="pastel-nav rounded-full px-6 py-3.5 flex items-center justify-between shadow-lg">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-sage to-lavender text-white flex items-center justify-center font-bold text-sm shadow-md">
                    AN
                </div>
                <span class="font-bold text-slateText text-sm sm:text-base tracking-tight">Auwalun Nisa’</span>
            </div>

            <!-- Desktop Menu -->
            <div class="hidden md:flex items-center space-x-8 text-sm font-medium text-slate-600">
                <a href="#about" class="hover:text-sage transition-colors">Tentang Saya</a>
                <a href="#skills" class="hover:text-sage transition-colors">Keahlian</a>
                <a href="#achievement" class="hover:text-sage transition-colors">Prestasi</a>
                <a href="#contact" class="hover:text-sage transition-colors">Kontak</a>
            </div>

            <div class="flex items-center space-x-3">
                <a href="#contact" class="hidden sm:inline-block px-5 py-2 rounded-full bg-sage text-white font-semibold text-xs hover:bg-[#5b7e6c] transition-all shadow-md">
                    Hubungi Saya
                </a>
                <button id="menu-btn" class="md:hidden text-slate-700 hover:text-sage focus:outline-none p-2">
                    <i class="fa-solid fa-bars text-lg"></i>
                </button>
            </div>
        </nav>

        <!-- Mobile Dropdown Menu -->
        <div id="mobile-menu" class="hidden md:hidden mt-2 pastel-card rounded-3xl p-6 space-y-4 text-center shadow-xl border border-sage/20">
            <a href="#about" class="block text-slate-700 hover:text-sage font-medium text-sm">Tentang Saya</a>
            <a href="#skills" class="block text-slate-700 hover:text-sage font-medium text-sm">Keahlian</a>
            <a href="#achievement" class="block text-slate-700 hover:text-sage font-medium text-sm">Prestasi</a>
            <a href="#contact" class="block text-slate-700 hover:text-sage font-medium text-sm">Kontak</a>
        </div>
    </header>

    <section class="relative pt-36 pb-20 lg:pt-44 lg:pb-32 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-sageLight text-sage text-xs font-semibold tracking-wide border border-sage/20">
                    <i class="fa-solid fa-graduation-cap"></i> S1 Pendidikan Teknologi Informasi
                </div>
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-slateText tracking-tight leading-tight">
                    Halo, Saya <br><span class="text-gradient">Auwalun Nisa’</span> ✨
                </h1>
                <p class="text-slate-600 text-base sm:text-lg max-w-xl mx-auto lg:mx-0 font-normal leading-relaxed">
                    Mahasiswa Baru Prodi Pendidikan Teknologi Informasi Universitas Negeri Surabaya.
                </p>
                <div class="flex flex-wrap items-center justify-center lg:justify-start gap-4 pt-2">
                    <a href="#about" class="px-7 py-3.5 rounded-full bg-sage text-white font-semibold text-sm hover:bg-[#5b7e6c] transition-all shadow-md flex items-center gap-2">
                        <i class="fa-solid fa-user"></i> Kenali Lebih Dekat
                    </a>
                </div>
            </div>

            <!-- Hero Avatar Card -->
            <div class="lg:col-span-5 flex justify-center">
                <div class="relative w-72 h-80 sm:w-80 sm:h-96 rounded-3xl pastel-card p-3 rotate-1 hover:rotate-0 transition-transform duration-500">
                    <div class="w-full h-full rounded-2xl bg-gradient-to-b from-sageLight via-lavenderLight to-peachLight flex flex-col items-center justify-center p-6 text-center border border-sage/20 relative overflow-hidden">
                        <div class="w-28 h-28 rounded-full bg-white text-sage flex items-center justify-center text-4xl font-bold shadow-xl mb-4 border-4 border-white z-10">
                            AN
                        </div>
                        <h3 class="text-xl font-bold text-slateText z-10">Auwalun Nisa’</h3>
                        <div class="mt-4 flex items-center gap-2 z-10 text-slate-600 text-xs bg-white/80 px-3 py-1.5 rounded-full shadow-sm">
                            <span class="w-2 h-2 rounded-full bg-sage animate-ping"></span>
                            <span>S1 PTI 2026</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="about" class="py-20 relative">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-sage bg-sageLight px-3 py-1 rounded-full border border-sage/20">Tentang Saya</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-slateText">Profil & Perjalanan Akademik</h2>
                <p class="text-slate-600 text-sm sm:text-base">Mengenal identitas, latar belakang pendidikan, serta pengalaman saya.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <!-- Biodata Card -->
                <div class="lg:col-span-5 pastel-card rounded-3xl p-8 space-y-6">
                    <div class="flex items-center space-x-4 border-b border-stone-200 pb-6">
                        <div class="w-16 h-16 rounded-2xl bg-lavenderLight text-lavender flex items-center justify-center text-2xl font-bold shadow-sm">
                            <i class="fa-solid fa-id-card"></i>
                        </div>
                        <div>
                            <h3 class="text-lg font-bold text-slateText">Auwalun Nisa’</h3>
                        </div>
                    </div>

                    <div class="space-y-4 text-sm">
                        <div class="flex justify-between items-center py-2 border-b border-stone-100">
                            <span class="text-slate-500 font-medium"><i class="fa-solid fa-hashtag mr-2 text-sky-600"></i> NIM:</span>
                            <span class="text-slateText font-semibold">26050974152</span>
                        </div>
                        <div class="flex justify-between items-center py-2 border-b border-stone-100">
                            <span class="text-slate-500 font-medium"><i class="fa-solid fa-graduation-cap mr-2 text-lavender"></i> Prodi:</span>
                            <span class="text-slateText font-semibold text-right">S1 Pendidikan Teknologi Informasi</span>
                        </div>
                       <div class="flex justify-between items-center py-2 border-b border-stone-100">
                            <span class="text-slate-500 font-medium"><i class="fa-solid fa-gear mr-2 text-sage"></i> Fakultas:</span>
                            <span class="text-slateText font-semibold">Fakultas Teknik</span> 
                       </div>
                        <div class="flex justify-between items-center py-2 border-b border-stone-100">
                            <span class="text-slate-500 font-medium"><i class="fa-solid fa-university mr-2 text-peach"></i> Universitas:</span>
                            <span class="text-slateText font-semibold">Universitas Negeri Surabaya</span>
                        </div>
                    </div>
                </div>
            
                <!-- Story -->
                <div class="lg:col-span-7 space-y-6">
                    <div class="pastel-card rounded-3xl p-8 space-y-4">
                        <h3 class="text-xl font-bold text-slateText flex items-center gap-2">
                            <i class="fa-solid fa-book-open text-sage"></i> Latar Belakang
                        </h3>
                        <p class="text-slate-600 text-sm leading-relaxed">
                            Halo! Saya <strong class="text-slateText">Auwalun Nisa’</strong>, mahasiswa baru Prodi Pendidikan Teknologi Informasi di Fakultas Teknik, Universitas Negeri Surabaya. Berawal dari ketertarikan yang kuat pada dunia teknologi saat menempuh pendidikan di SMAN 1 Gondang Mojokerto, saya kini mendedikasikan diri untuk mengeksplorasi bagaimana teknologi dapat mentransformasi dunia terutama dalampendidikan. Saya percaya bahwa integrasi teknologi, kecerdasan buatan, dan pembelajaran digital adalah kunci penting dalam mencetak generasi unggul untuk mendukung Visi Indonesia Emas 2045.
                        </p>
                        <p class="text-slate-600 text-sm leading-relaxed">
                            Saat ini, kegiatan saya berpusat pada perkuliahan, memperdalam pemahaman pada materi algoritma&pemrograman, sistem operasi, dan basis data, serta mengasah hardskill dan softskill agar kelak dapat berkontribusi positif dalam dunia teknologi dan pendidikan.
                        </p>
                    </div>
                </div>

            <div class="lg:col-span-full">
                <!-- Hobbies -->
                    <div class="pastel-card rounded-3xl p-8 space-y-4">
                        <h3 class="text-xl font-bold text-slateText flex items-center gap-2">
                            <i class="fa-solid fa-palette text-peach"></i> Aktivitas & Hobi
                        </h3>
                        <p class="text-slate-600 text-sm leading-relaxed">
                         Selain mendalami dunia teknologi, saya memiliki hobi sebagai berikut:
                        </p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-2">
                        <div class="p-4 rounded-2xl bg-sageLight/60 border border-sage/20 text-center space-y-2">
                            <div class="w-10 h-10 mx-auto rounded-full bg-white text-sage flex items-center justify-center text-sm font-bold shadow-sm">
                                <i class="fa-solid fa-microphone-lines"></i>
                            </div>
                                <h4 class="font-bold text-slateText text-xs">Menyanyi</h4>
                                <p class="text-[11px] text-slate-500">Saya suka semua genre musik, namun saya hanya mengetahui beberapa lagu.</p>
                        </div>
                        <div class="p-4 rounded-2xl bg-peachLight border border-peach/20 text-center space-y-2">
                            <div class="w-10 h-10 mx-auto rounded-full bg-white text-peach flex items-center justify-center text-sm font-bold shadow-sm">
                                <i class="fa-solid fa-music"></i>
                            </div>
                            <h4 class="font-bold text-slateText text-xs">Dance</h4>
                            <p class="text-[11px] text-slate-500">Selain menyanyi, saya juga suka menari dan mengekspresikan diri melalui gerakan tubuh. Namun, saya masih terlalu kaku dalam menari.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="py-20 relative bg-[#F2EFE9]/50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-lavender bg-lavenderLight px-3 py-1 rounded-full border border-lavender/20">What I Can Do</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-slateText">Keahlian & Kemampuan</h2>
                <p class="text-slate-600 text-sm sm:text-base">Pengalaman dalam organisasi dan kerja sama tim.</p>
            </div>
        
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 max-w-4xl mx-auto">
            <!-- Card Leadership -->
            <div class="p-4 rounded-2xl bg-sageLight/60 border border-sage/20 space-y-2">
                <div class="flex items-center gap-2 text-sage font-bold text-xs">
                    <i class="fa-solid fa-user-tie text-sm"></i> Leadership
                </div>
                <p class="text-[11px] text-slate-500">
                    Pernah mengemban amanah sebagai Sekretaris 1 dalam organisasi, memimpin koordinasi kesekretariatan, serta mengatur jalannya administrasi program kerja.
                </p>
            </div>

            <!-- Card Teamwork -->
            <div class="p-4 rounded-2xl bg-peachLight border border-peach/20 space-y-2">
                <div class="flex items-center gap-2 text-peach font-bold text-xs">
                    <i class="fa-solid fa-handshake text-sm"></i> Teamwork
                </div>
                <p class="text-[11px] text-slate-500">
                    Terbiasa berkolaborasi secara aktif dalam tugas kelompok maupun kepengurusan organisasi untuk mencapai tujuan bersama dengan komunikasi yang efektif.
                </p>
            </div>
        </div>

    </div>
</div>

    <section id="achievement" class="py-20 relative">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-peach bg-peachLight px-3 py-1 rounded-full border border-peach/20">Achievement</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-slateText">Pencapaian & Pengalaman</h2>
                <p class="text-slate-600 text-sm sm:text-base">Jejak prestasi akademik dan pengembangan diri.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 max-w-4xl mx-auto">
                <!-- Achievement 1 -->
                <div class="pastel-card rounded-3xl p-6 space-y-3">
                    <div class="flex items-center justify-between">
                        <span class="text-xs font-bold text-sage bg-sageLight px-3 py-1 rounded-full">2025</span>
                        <span class="text-xs text-slate-500 font-medium">SMAN 1 Gondang</span>
                    </div>
                    <h3 class="text-lg font-bold text-slateText">Peserta OSN Fisika Tingkat Kabupaten</h3>
                    <p class="text-slate-600 text-xs leading-relaxed">
                        Berpartisipasi dalam Olimpiade Sains Nasional (OSN) bidang Fisika tingkat kabupaten, mengasah kemampuan analisis, pemecahan masalah kompleks, dan logika sains.
                    </p>
                </div>

                <!-- Achievement 2 -->
                <div class="pastel-card rounded-3xl p-6 space-y-3">
                    <div class="flex items-center justify-between">
                        <span class="text-xs font-bold text-lavender bg-lavenderLight px-3 py-1 rounded-full">2024/2025</span>
                        <span class="text-xs text-slate-500 font-medium">SMAN 1 Gondang</span>
                    </div>
                    <h3 class="text-lg font-bold text-slateText">Sekretaris 1 UKKI</h3>
                    <p class="text-slate-600 text-xs leading-relaxed">
                        Menjabat sebagai Sekretaris 1 Unit Kegiatan Kerohanian Islam (UKKI), bertanggung jawab atas administrasi dan koordinasi kegiatan organisasi.
                    </p>
                </div>

                <!-- Achievement 3 -->
                <div class="pastel-card rounded-3xl p-6 space-y-3">
                    <div class="flex items-center justify-between">
                        <span class="text-xs font-bold text-peach bg-peachLight px-3 py-1 rounded-full">2025</span>
                        <span class="text-xs text-slate-500 font-medium">SMAN 1 Gondang</span>
                    </div>
                    <h3 class="text-lg font-bold text-slateText">Juara 2 OMF</h3>
                    <p class="text-slate-600 text-xs leading-relaxed">
                        Meraih Juara 2 dalam Olimpiade Master Fisika (OMF) pada babak penyisihan, yang diselenggarakan oleh Student Olympiad dalam rangka persiapan menghadapi Olimpiade Sains Nasional (OSN) tingkat kabupaten.
                    </p>
                </div>

                <!-- Achievement 4 -->
                <div class="pastel-card rounded-3xl p-6 space-y-3">
                    <div class="flex items-center justify-between">
                        <span class="text-xs font-bold text-emerald-600 bg-emerald-50 px-3 py-1 rounded-full">2024-2025</span>
                        <span class="text-xs text-slate-500 font-medium">SMAN 1 Gondang</span>
                    </div>
                    <h3 class="text-lg font-bold text-slateText">Peserta Lomba Banjari</h3>
                    <p class="text-slate-600 text-xs leading-relaxed">
                        Menjadi peserta dari beberapa lomba Banjari tingkat kabupaten, mengembangkan kemampuan percaya diri, koordinasi tim, dan apresiasi terhadap seni musik islam.
                    </p>
                </div>
            </div>
        </div>
    </section>


    <section id="contact" class="py-20 relative">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-sage bg-sageLight px-3 py-1 rounded-full border border-sage/20">Contact</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-slateText">Mari Terhubung</h2>
                <p class="text-slate-600 text-sm sm:text-base">Punya pertanyaan, tawaran kolaborasi, atau ingin berdiskusi? Jangan ragu untuk menghubungi saya.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <!-- Social Links -->
                <div class="lg:col-span-5 space-y-4">
                    <a href="mailto:auwalun.nisa@mhs.unesa.ac.id" class="pastel-card rounded-3xl p-5 flex items-center gap-4 hover:border-sage transition-all block">
                        <div class="w-12 h-12 rounded-2xl bg-sageLight text-sage flex items-center justify-center text-xl shrink-0 shadow-sm">
                            <i class="fa-solid fa-envelope"></i>
                        </div>
                        <div>
                            <span class="text-[11px] text-slate-500 block font-medium">Email</span>
                            <span class="text-xs sm:text-sm text-slateText font-semibold">26050974152@mhs.unesa.ac.id</span>
                            <span class="text-xs sm:text-sm text-slateText font-semibold">auwalunnisa086@gmail.com</span>
                        </div>
                    </a>

                    <a href="https://linkedin.com" target="_blank" class="pastel-card rounded-3xl p-5 flex items-center gap-4 hover:border-lavender transition-all block">
                        <div class="w-12 h-12 rounded-2xl bg-lavenderLight text-lavender flex items-center justify-center text-xl shrink-0 shadow-sm">
                            <i class="fa-brands fa-linkedin"></i>
                        </div>
                        <div>
                            <span class="text-[11px] text-slate-500 block font-medium">LinkedIn Profile</span>
                            <span class="text-xs sm:text-sm text-slateText font-semibold">linkedin.com/in/auwalun-nisa-a2316b441</span>
                        </div>
                    </a>

                    <a href="https://github.com" target="_blank" class="pastel-card rounded-3xl p-5 flex items-center gap-4 hover:border-slate-400 transition-all block">
                        <div class="w-12 h-12 rounded-2xl bg-stone-100 text-slate-700 flex items-center justify-center text-xl shrink-0 shadow-sm">
                            <i class="fa-brands fa-github"></i>
                        </div>
                        <div>
                            <span class="text-[11px] text-slate-500 block font-medium">GitHub Repository</span>
                            <span class="text-xs sm:text-sm text-slateText font-semibold">github.com/awlnnisaa</span>
                        </div>
                    </a>

                    <a href="https://instagram.com" target="_blank" class="pastel-card rounded-3xl p-5 flex items-center gap-4 hover:border-peach transition-all block">
                        <div class="w-12 h-12 rounded-2xl bg-peachLight text-peach flex items-center justify-center text-xl shrink-0 shadow-sm">
                            <i class="fa-brands fa-instagram"></i>
                        </div>
                        <div>
                            <span class="text-[11px] text-slate-500 block font-medium">Instagram Account</span>
                            <span class="text-xs sm:text-sm text-slateText font-semibold">@awlnnisaa</span>
                        </div>
                    </a>

                    <button onclick="downloadResume()" class="w-full py-3.5 rounded-full bg-sage text-white font-bold text-xs uppercase tracking-widest hover:bg-[#5b7e6c] transition-all shadow-md flex items-center justify-center gap-2">
                        <i class="fa-solid fa-download"></i> Unduh CV / Resume
                    </button>
                </div>

                <!-- Message Form -->
                <div class="lg:col-span-7">
                    <form id="contact-form" onsubmit="handleContactSubmit(event)" class="pastel-card rounded-3xl p-8 space-y-4">
                        <h3 class="text-lg font-bold text-slateText mb-2">Kirim Pesan Singkat</h3>
                        <div>
                            <label class="block text-xs font-medium text-slate-600 mb-1.5">Nama Anda:</label>
                            <input type="text" id="sender-name" required placeholder="Masukkan nama..." class="w-full px-4 py-3 rounded-2xl bg-stone-50 border border-stone-200 text-slateText placeholder-stone-400 focus:outline-none focus:border-sage text-xs sm:text-sm">
                        </div>
                        <div>
                            <label class="block text-xs font-medium text-slate-600 mb-1.5">Alamat Email:</label>
                            <input type="email" id="sender-email" required placeholder="nama@domain.com" class="w-full px-4 py-3 rounded-2xl bg-stone-50 border border-stone-200 text-slateText placeholder-stone-400 focus:outline-none focus:border-sage text-xs sm:text-sm">
                        </div>
                        <div>
                            <label class="block text-xs font-medium text-slate-600 mb-1.5">Pesan:</label>
                            <textarea id="sender-msg" rows="4" required placeholder="Tuliskan pesan Anda di sini..." class="w-full px-4 py-3 rounded-2xl bg-stone-50 border border-stone-200 text-slateText placeholder-stone-400 focus:outline-none focus:border-sage text-xs sm:text-sm"></textarea>
                        </div>
                        <button type="submit" class="w-full py-3.5 rounded-full bg-sage text-white font-semibold text-xs uppercase tracking-widest hover:bg-[#5b7e6c] transition-all shadow-md flex items-center justify-center gap-2">
                            <i class="fa-solid fa-paper-plane"></i> Kirim Pesan
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <div id="toast-box" class="fixed bottom-6 right-6 z-50 transform translate-y-32 opacity-0 transition-all duration-300 pastel-card border border-sage/30 p-4 rounded-2xl flex items-center gap-3 shadow-2xl bg-white">
        <div class="w-9 h-9 rounded-full bg-sageLight text-sage flex items-center justify-center text-sm font-bold shadow-sm">
            <i class="fa-solid fa-check"></i>
        </div>
        <div>
            <span id="toast-title" class="block font-bold text-slateText text-xs">BERHASIL</span>
            <span id="toast-desc" class="text-[11px] text-slate-600">Pesan Anda telah terkirim.</span>
        </div>
    </div>

    <footer class="py-8 bg-white border-t border-stone-200 text-center text-slate-500 text-xs">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4">
            <p>&copy;2026 Auwalun Nisa’</p>
            <div class="flex items-center space-x-3 text-sage font-medium">
                <span>S1 PTI — FT — UNESA</span>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        mobileMenu.querySelectorAll('a').forEach(l => l.addEventListener('click', () => mobileMenu.classList.add('hidden')));

        // Toast notification helper
        function showToast(title, desc) {
            const toast = document.getElementById('toast-box');
            document.getElementById('toast-title').innerText = title;
            document.getElementById('toast-desc').innerText = desc;
            toast.classList.remove('translate-y-32', 'opacity-0');
            setTimeout(() => {
                toast.classList.add('translate-y-32', 'opacity-0');
            }, 4000);
        }

        function handleContactSubmit(e) {
            e.preventDefault();
            const name = document.getElementById('sender-name').value;
            showToast("PESAN TERKIRIM", `Terima kasih ${name}, pesan Anda berhasil dikirim.`);
            document.getElementById('contact-form').reset();
        }

        function downloadResume() {
            showToast("MENGUNDUH CV", "Mengunduh dokumen CV_Auwalun_Nisa_PTI_UNESA.pdf...");
        }
    </script>
</body>
</html>
