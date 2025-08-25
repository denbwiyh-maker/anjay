<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title class="h1">Portal Berita Terkini</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans:wght@400;700&display=swap');
        
        body {
            font-family: 'Noto Sans', sans-serif;
            line-height: 1.6;
        }
        
        .navbar {
            background: linear-gradient(90deg, #1a365d 0%, #153e75 100%);
        }
        
        .breaking-news {
            background-color: #e53e3e;
            animation: pulse 2s infinite;
        }
        
        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }
        
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.8; }
            100% { opacity: 1; }
        }
        
        .category-tag {
            transition: all 0.3s ease;
        }
        
        .category-tag:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header/Navbar -->
    <header class="navbar text-white shadow-md">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <img src="4c9ee980-e78a-4598-bae0-bf40b18cc544.jfif" alt="Logo portal berita berupa lingkaran dengan ikon surat kabar berwarna putih" class="h-10">
                <h1 class="text-xl font-bold">BeritaHariIni</h1>
            </div>
                    <li><a href="#" class="hover:text-blue-200 font-medium">Beranda</a></li>
                    <li><a href="#" class="hover:text-blue-200">Nasional</a></li>
                    <li><a href="#" class="hover:text-blue-200">Internasional</a></li>
                    <li><a href="#" class="hover:text-blue-200">Ekonomi</a></li>
                    <li><a href="#" class="hover:text-blue-200">Olahraga</a></li>
                    <li><a href="#" class="hover:text-blue-200">Teknologi</a></li>
                </ul>
            </nav>
            
            <div class="flex items-center space-x-4">
                <div class="relative">
                    <input type="text" placeholder="Cari berita..." class="py-1 px-3 rounded-full text-gray-800 text-sm w-40 md:w-64">
                    <button class="absolute right-2 top-1/2 transform -translate-y-1/2 text-gray-500">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                        </svg>
                    </button>
                </div>
                <button class="md:hidden">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>
    </header>

    <!-- Breaking News Banner -->
    <div class="breaking-news text-white py-2 px-4">
        <div class="container mx-auto flex items-center">
            <span class="font-bold mr-4">BREAKING:</span>
            <marquee>Pemerintah umumkan paket stimulus ekonomi baru untuk UMKM | Kasus COVID-19 turun 20% minggu ini | Timnas Indonesia juara turnamen persahabatan</marquee>
        </div>
    </div>

    <main class="container mx-auto px-4 py-8">
        <!-- Featured News -->
        <section class="mb-12">
            <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ea5062a2-7145-4588-b74a-2710af682e13.png" alt="Presiden Indonesia sedang memberikan pidato di depan kerumunan dengan bendera merah putih berkibar" class="w-full h-64 md:h-96 object-cover">
                <div class="p-6">
                    <span class="inline-block px-3 py-1 bg-red-100 text-red-800 rounded-full text-sm font-semibold mb-2 category-tag">NASIONAL</span>
                    <h2 class="text-2xl md:text-3xl font-bold mb-3">Pemerintah Umumkan Rencana Pembangunan Infrastruktur Besar-besaran di Tahun 2023</h2>
                    <p class="text-gray-600 mb-4">Pemerintah mengalokasikan anggaran Rp 500 triliun untuk pembangunan infrastruktur di seluruh Indonesia, termasuk jalan tol, bandara, dan pelabuhan baru yang akan mendorong pertumbuhan ekonomi nasional.</p>
                    <div class="flex items-center text-sm text-gray-500">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ea2ee5e5-938d-4e2d-8b1c-120f3af5e14a.png" alt="Foto penulis berita dengan kemeja formal" class="w-6 h-6 rounded-full mr-2">
                        <span>John Doe</span>
                        <span class="mx-2">•</span>
                        <span>2 jam yang lalu</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- News Grid -->
        <section class="mb-12">
            <div class="flex justify-between items-center mb-6 border-b pb-2">
                <h2 class="text-xl font-bold">Berita Terkini</h2>
                <a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Lihat Semua →</a>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- News Card 1 -->
                <article class="news-card bg-white rounded-lg shadow-md overflow-hidden transition duration-300">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/129f461f-968d-4594-ba52-e862d37ff8dc.png" alt="Ilustrasi teknologi 5G dengan latar belakang jaringan digital berwarna biru" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <span class="inline-block px-2 py-1 bg-blue-100 text-blue-800 rounded-full text-xs font-semibold mb-2 category-tag">TEKNOLOGI</span>
                        <h3 class="text-lg font-semibold mb-2">Operator Telekomunikasi Siap Luncurkan Jaringan 5G di Indonesia</h3>
                        <p class="text-gray-600 text-sm mb-3">Empat operator telekomunikasi besar di Indonesia telah menyelesaikan uji coba jaringan 5G dan siap meluncurkan layanan komersial pada kuartal kedua tahun ini.</p>
                        <div class="flex items-center text-xs text-gray-500">
                            <span>Jane Smith</span>
                            <span class="mx-2">•</span>
                            <span>5 jam yang lalu</span>
                        </div>
                    </div>
                </article>
                
                <!-- News Card 2 -->
                <article class="news-card bg-white rounded-lg shadow-md overflow-hidden transition duration-300">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/e7318149-35d7-48a3-bb7f-428b50cc2b6a.png" alt="Pemain sepak bola Indonesia sedang merayakan gol dalam pertandingan internasional" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <span class="inline-block px-2 py-1 bg-green-100 text-green-800 rounded-full text-xs font-semibold mb-2 category-tag">OLAHRAGA</span>
                        <h3 class="text-lg font-semibold mb-2">Timnas Indonesia Juara Turnamen Piala AFF 2023</h3>
                        <p class="text-gray-600 text-sm mb-3">Tim nasional Indonesia berhasil mengalahkan Malaysia dengan skor 3-1 di final Piala AFF 2023, membawa pulang trofi setelah 12 tahun masa tunggu.</p>
                        <div class="flex items-center text-xs text-gray-500">
                            <span>Alex Wong</span>
                            <span class="mx-2">•</span>
                            <span>8 jam yang lalu</span>
                        </div>
                    </div>
                </article>
                
                <!-- News Card 3 -->
                <article class="news-card bg-white rounded-lg shadow-md overflow-hidden transition duration-300">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/29fd6bbc-d57e-420c-91e4-c40db4032ebf.png" alt="Harga saham di monitor digital dengan grafik yang sedang naik" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <span class="inline-block px-2 py-1 bg-yellow-100 text-yellow-800 rounded-full text-xs font-semibold mb-2 category-tag">EKONOMI</span>
                        <h3 class="text-lg font-semibold mb-2">IHSG Naik 2% di Penutupan Perdagangan Hari Ini</h3>
                        <p class="text-gray-600 text-sm mb-3">Indeks Harga Saham Gabungan (IHSG) menguat 2% ditutup pada level 7.250, dipimpin oleh saham-saham sektor perbankan dan properti yang mencatat kenaikan signifikan.</p>
                        <div class="flex items-center text-xs text-gray-500">
                            <span>Michael Tan</span>
                            <span class="mx-2">•</span>
                            <span>10 jam yang lalu</span>
                        </div>
                    </div>
                </article>
            </div>
        </section>

        <!-- News Categories -->
        <section class="mb-12">
            <div class="flex justify-between items-center mb-6 border-b pb-2">
                <h2 class="text-xl font-bold">Kategori Berita</h2>
                <a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Lihat Semua →</a>
            </div>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <a href="#" class="category-card bg-blue-50 hover:bg-blue-100 rounded-lg p-4 text-center transition">
                    <div class="bg-blue-100 w-12 h-12 mx-auto rounded-full flex items-center justify-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9" />
                        </svg>
                    </div>
                    <h3 class="font-medium">Internasional</h3>
                </a>
                
                <a href="#" class="category-card bg-red-50 hover:bg-red-100 rounded-lg p-4 text-center transition">
                    <div class="bg-red-100 w-12 h-12 mx-auto rounded-full flex items-center justify-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-red-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                    <h3 class="font-medium">Nasional</h3>
                </a>
                
                <a href="#" class="category-card bg-green-50 hover:bg-green-100 rounded-lg p-4 text-center transition">
                    <div class="bg-green-100 w-12 h-12 mx-auto rounded-full flex items-center justify-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z" />
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6z" />
                        </svg>
                    </div>
                    <h3 class="font-medium">Bisnis</h3>
                </a>
                
                <a href="#" class="category-card bg-purple-50 hover:bg-purple-100 rounded-lg p-4 text-center transition">
                    <div class="bg-purple-100 w-12 h-12 mx-auto rounded-full flex items-center justify-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-purple-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" />
                        </svg>
                    </div>
                    <h3 class="font-medium">Teknologi</h3>
                </a>
            </div>
        </section>

        <!-- Popular News -->
        <section>
            <div class="flex justify-between items-center mb-6 border-b pb-2">
                <h2 class="text-xl font-bold">Berita Populer</h2>
                <a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Lihat Semua →</a>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <article class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="p-4">
                        <div class="flex items-start">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/da99e767-df14-4064-8d37-e00d41ed6b3f.png" alt="Foto profil menteri kesehatan indonesia" class="w-16 h-16 rounded-full object-cover mr-4">
                            <div>
                                <span class="inline-block px-2 py-1 bg-red-100 text-red-800 rounded-full text-xs font-semibold mb-1">KESEHATAN</span>
                                <h3 class="text-lg font-semibold">Menteri Kesiapan Hadapi Varian Baru COVID-19</h3>
                                <div class="flex items-center text-xs text-gray-500 mt-2">
                                    <span>22.5K views</span>
                                    <span class="mx-2">•</span>
                                    <span>3 hari lalu</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </article>
                
                <article class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="p-4">
                        <div class="flex items-start">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/434a5420-bac9-408d-bc3a-922a3d113cd6.png" alt="Pemandangan gunung tertutup salju dengan iklim dingin" class="w-16 h-16 rounded-full object-cover mr-4">
                            <div>
                                <span class="inline-block px-2 py-1 bg-blue-100 text-blue-800 rounded-full text-xs font-semibold mb-1">LINGKUNGAN</span>
                                <h3 class="text-lg font-semibold">Perubahan Iklim: Es di Kutub Mencair Lebih Cepat dari Perkiraan</h3>
                                <div class="flex items-center text-xs text-gray-500 mt-2">
                                    <span>18.7K views</span>
                                    <span class="mx-2">•</span>
                                    <span>5 hari lalu</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </article>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-lg font-bold mb-4">BeritaHariIni</h3>
                    <p class="text-gray-400 text-sm">Portal berita terkini dan terpercaya yang menyajikan informasi aktual dari dalam dan luar negeri.</p>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Kategori</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Nasional</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Internasional</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Ekonomi</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Olahraga</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Teknologi</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Tentang Kami</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Profil Perusahaan</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Kontak</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Karier</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Iklan</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Kebijakan</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Kebijakan Privasi</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Syarat & Ketentuan</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Pedoman Media Siber</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center">
                    <p class="text-gray-400 text-sm">© 2023 BeritaHariIni. All rights reserved.</p>
                    <div class="flex space-x-4 mt-4 md:mt-0">
                        <a href="#" class="text-gray-400 hover:text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z" />
                            </svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" />
                            </svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" />
                            </svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z" />
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.querySelector('header button').addEventListener('click', function() {
            const nav = document.querySelector('header nav');
            nav.classList.toggle('hidden');
            nav.classList.toggle('block');
        });

        // Search functionality
        document.querySelector('.relative button').addEventListener('click', function() {
            const searchTerm = document.querySelector('.relative input').value;
            if(searchTerm.trim() !== '') {
                alert('Anda mencari: ' + searchTerm);
                // In a real application, this would perform an AJAX request
            }
        });

        // Simulate loading popular news
        setTimeout(function() {
            const popularNews = document.querySelectorAll('.popular-news-loading');
            popularNews.forEach(news => {
                news.classList.remove('animate-pulse');
                news.classList.remove('bg-gray-200');
            });
        }, 1500);
    </script>
</body>
</html>

```