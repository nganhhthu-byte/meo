# meo
<!DOCTYPE html>
<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meo Flowers | Korean Floral & Crochet Boutique</title>
    <meta name="description" content="Meo Flowers - Tiệm hoa tươi và đồ len crochet phong cách Hàn Quốc tại Huế. Chuyên cung cấp hoa sự kiện, hoa tốt nghiệp và quà tặng thiết kế riêng với thông điệp Yêu thương lan tỏa.">
    <meta name="keywords" content="Meo Flowers, tiệm hoa Huế, hoa tươi Huế, hoa crochet, hoa len, florist Hue, hoa Hàn Quốc">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --bg-color: #fff5f7;
            --text-color: #2f4f4f;
        }
        body { 
            font-family: 'Montserrat', sans-serif; 
            color: var(--text-color); 
            background-color: var(--bg-color); 
        }
        .font-serif { font-family: 'Playfair Display', serif; }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 5px; }
        ::-webkit-scrollbar-track { background: var(--bg-color); }
        ::-webkit-scrollbar-thumb { background: #2f4f4f; border-radius: 10px; }

        /* Animation Classes */
        .reveal { opacity: 0; transform: translateY(30px); transition: all 0.8s ease-out; }
        .reveal.active { opacity: 1; transform: translateY(0); }

        .flower-card:hover .img-zoom { transform: scale(1.05); }
        .img-zoom { transition: transform 1.2s cubic-bezier(0.2, 0, 0.2, 1); }

        .nav-underline { position: relative; }
        .nav-underline::after {
            content: ''; position: absolute; width: 0; height: 1px;
            bottom: -2px; left: 0; background-color: var(--text-color);
            transition: width 0.3s ease;
        }
        .nav-underline:hover::after { width: 100%; }

        /* Floating Contact Animation */
        @keyframes pulse {
            0% { transform: scale(1); box-shadow: 0 0 0 0 rgba(47, 79, 79, 0.2); }
            70% { transform: scale(1.05); box-shadow: 0 0 0 10px rgba(47, 79, 79, 0); }
            100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(47, 79, 79, 0); }
        }
        .btn-pulse { animation: pulse 2s infinite; }
    </style>
</head>
<body class="overflow-x-hidden">

    <nav class="fixed top-0 w-full z-[100] bg-[#fff5f7]/90 backdrop-blur-md border-b border-gray-100 px-6 py-4 md:px-12 flex justify-between items-center">
        <div class="flex items-center gap-4">
            <img src="https://i.ibb.co/4nTZRpHz/logo.jpg" 
                 alt="Meo Flowers Logo" class="w-10 h-10 rounded-full object-cover shadow-sm border border-gray-100">
            <span class="text-xl font-serif font-semibold tracking-[0.2em] uppercase">Meo Flowers</span>
        </div>
        
        <div class="hidden md:flex space-x-10 text-[10px] tracking-[0.25em] uppercase font-medium">
            <a href="#home" class="nav-underline">Home</a>
            <a href="#booking" class="nav-underline">Menu & Price</a>
            <a href="#events" class="nav-underline">Collections</a>
            <a href="#contact" class="nav-underline">Contact</a>
        </div>

        <div class="md:hidden">
            <i class="fa-solid fa-bars-staggered text-xl cursor-pointer" id="menuToggle"></i>
        </div>
    </nav>

    <section id="home" class="relative h-screen flex flex-col justify-center items-center text-center px-6">
        <div class="reveal">
            <img src="https://i.ibb.co/4nTZRpHz/logo.jpg" 
            alt="Meo Flowers Logo" class="w-32 h-32 md:w-48 md:h-48 rounded-full object-cover mx-auto mb-8 shadow-lg border-4 border-white">
            
            <span class="text-[11px] tracking-[0.5em] uppercase opacity-60 mb-6 block">— Seoul Inspired Florist —</span>
            <h1 class="font-serif italic text-6xl md:text-8xl mb-8 font-light leading-tight">Meo <br> Flowersandcrochet</h1>
            <p class="max-w-xl mx-auto text-xs md:text-sm tracking-[0.2em] leading-loose opacity-70 uppercase mb-12">
                Hoa trao tay - Yêu thương lan tỏa.
            </p>
            <div class="flex flex-col md:flex-row gap-6 justify-center">
                <a href="#booking" class="px-10 py-4 border border-[#2f4f4f] text-[10px] tracking-[0.3em] uppercase hover:bg-[#2f4f4f] hover:text-white transition-all duration-500">Xem Bảng Giá</a>
                <a href="tel:0941190148" class="px-10 py-4 bg-[#2f4f4f] text-white text-[10px] tracking-[0.3em] uppercase hover:bg-white hover:text-[#2f4f4f] border border-[#2f4f4f] transition-all duration-500">Liên Hệ Ngay</a>
            </div>
        </div>
    </section>

    <section id="booking" class="py-32 bg-white/30 px-6 shadow-inner">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-20 reveal">
                <h2 class="font-serif text-4xl italic mb-4">Gói Trọn Cảm Xúc</h2>
                <div class="w-12 h-[1px] bg-[#2f4f4f] mx-auto mb-6 opacity-30"></div>
                <p class="text-[10px] tracking-[0.4em] uppercase opacity-60">Chọn hoa theo tầm giá & nhu cầu của bạn</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
                <div class="reveal" style="transition-delay: 0.2s;">
                    <h3 class="text-xs tracking-[0.3em] uppercase font-semibold mb-10 pb-4 border-b border-[#2f4f4f]/10 flex justify-between items-center">
                        <span>Ngân sách</span>
                        <i class="fa-solid fa-chevron-right text-[8px]"></i>
                    </h3>
                    <div class="space-y-5">
                        <a href="#" class="group flex justify-between items-center p-6 bg-white/50 hover:bg-[#2f4f4f] hover:text-white transition-all duration-500" data-event="mini">
                            <span class="font-serif italic text-xl">Mini Collection</span>
                            <span class="text-sm tracking-widest font-light opacity-60">120.000 — 200.000</span>
                        </a>
                        <a href="#" class="group flex justify-between items-center p-6 bg-white/50 hover:bg-[#2f4f4f] hover:text-white transition-all duration-500" data-event="daily">
                            <span class="font-serif italic text-xl">Daily Collection</span>
                            <span class="text-sm tracking-widest font-light opacity-60">250.000 — 350.000</span>
                        </a>
                        <a href="#" class="group flex justify-between items-center p-6 bg-white/50 hover:bg-[#2f4f4f] hover:text-white transition-all duration-500" data-event="signature">
                            <span class="font-serif italic text-xl">Signature Collection</span>
                            <span class="text-sm tracking-widest font-light opacity-60">400.000 — 600.000</span>
                        </a>
                        <a href="#" class="group flex justify-between items-center p-6 bg-white/50 hover:bg-[#2f4f4f] hover:text-white transition-all duration-500" data-event="luxury">
                            <span class="font-serif italic text-xl">Luxury Collection</span>
                            <span class="text-sm tracking-widest font-light opacity-60">650.000 — 1.000.000</span>
                        </a>
                        <a href="#" class="group flex justify-between items-center p-6 bg-white/50 hover:bg-[#2f4f4f] hover:text-white transition-all duration-500" data-event="premium">
                            <span class="font-serif italic text-xl">Premium Collection</span>
                            <span class="text-sm tracking-widest font-light opacity-60">Trên 1.200.000</span>
                        </a>
                    </div>
                </div>

                <div class="reveal" style="transition-delay: 0.4s;">
                    <h3 class="text-xs tracking-[0.3em] uppercase font-semibold mb-10 pb-4 border-b border-[#2f4f4f]/10 flex justify-between items-center">
                        <span>Sự kiện</span>
                        <i class="fa-solid fa-chevron-right text-[8px]"></i>
                    </h3>
                    <div class="grid grid-cols-2 gap-9">
                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="valentine">
                            <i class="fa-solid fa-heart-pulse mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Valentine (14/2)</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="graduation">
                            <i class="fa-solid fa-graduation-cap mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Happy Graduation</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="opening">
                            <i class="fa-solid fa-store mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Khai trương</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="wedding">
                            <i class="fa-solid fa-champagne-glasses mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Happy wedding</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="womensday">
                            <i class="fa-solid fa-venus mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Women's day</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="boysday">
                            <i class="fa-solid fa-mars mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Boy's day</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="trungthu">
                            <i class="fa-solid fa-moon mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Trung thu</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="noel">
                            <i class="fa-solid fa-snowflake mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Noel</p>
                        </a>

                        <a href="#" class="border border-[#2f4f4f]/10 bg-white/30 p-6 text-center hover:border-[#2f4f4f] transition-all group" data-event="blackwhite">
                            <i class="fa-solid fa-palette mb-3 opacity-30 group-hover:opacity-100 transition-opacity"></i>
                            <p class="text-[10px] tracking-widest uppercase">Black & White</p>
                        </a>

                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="events" class="py-24 bg-white">
    <div class="max-w-[1400px] mx-auto px-6">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            
            <div class="space-y-6">
                <div class="overflow-hidden relative group h-[600px] reveal">
                    <img src="https://i.ibb.co/JWzDNfHv/event.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/20 group-hover:bg-black/40 transition-all"></div>
                    <div class="absolute bottom-10 left-10 text-white">
                        <h4 class="font-serif text-4xl italic mb-2">Event Decor</h4>
                        <p class="text-[10px] tracking-[0.4em] uppercase opacity-80">Trang trí sự kiện cao cấp</p>
                    </div>
                </div>

                <div class="overflow-hidden relative group h-[300px] reveal" style="transition-delay: 0.2s;">
                    <img src="https://i.ibb.co/WW6HxM2M/noel.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/10 group-hover:bg-black/40 flex items-center justify-center transition-all opacity-0 group-hover:opacity-100">
                        <span class="text-white text-[10px] tracking-[0.4em] uppercase border border-white px-6 py-2">Noel</span>
                    </div>
                </div>
            </div>

            <div class="space-y-6 md:mt-12">
                <div class="overflow-hidden relative group h-[300px] reveal">
                    <img src="https://i.ibb.co/wZvgKNYQ/women-s-day.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/10 group-hover:bg-black/40 flex items-center justify-center transition-all opacity-0 group-hover:opacity-100">
                        <span class="text-white text-[10px] tracking-[0.4em] uppercase border border-white px-6 py-2">8/3 & 20/10</span>
                    </div>
                </div>

                <div class="overflow-hidden relative group h-[500px] reveal" style="transition-delay: 0.2s;">
                    <img src="https://i.ibb.co/kgJK8ZFN/buffet-hoa.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/20 group-hover:bg-black/40 transition-all"></div>
                    <div class="absolute bottom-10 left-10 text-white">
                        <h4 class="font-serif text-4xl italic mb-2">Buffet Hoa</h4>
                        <p class="text-[10px] tracking-[0.4em] uppercase opacity-80">Tự tay chọn hoa theo ý thích</p>
                    </div>
                </div>

                <div class="overflow-hidden relative group h-[350px] reveal" style="transition-delay: 0.3s;">
                    <img src="https://i.ibb.co/GfdT3gk7/khai-tr-ng.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/10 group-hover:bg-black/40 flex items-center justify-center transition-all opacity-0 group-hover:opacity-100">
                        <span class="text-white text-[10px] tracking-[0.4em] uppercase border border-white px-6 py-2">Khai Trương</span>
                    </div>
                </div>
            </div>

            <div class="space-y-6">
                <div class="overflow-hidden relative group h-[500px] reveal">
                    <img src="https://i.ibb.co/b5QDZWSy/graduation.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/20 group-hover:bg-black/40 transition-all"></div>
                    <div class="absolute bottom-10 left-10 text-white">
                        <h4 class="font-serif text-4xl italic mb-2">Graduation</h4>
                        <p class="text-[10px] tracking-[0.4em] uppercase opacity-80">Bảo vệ khoá luận & Lễ tốt nghiệp</p>
                    </div>
                </div>

                <div class="overflow-hidden relative group h-[300px] reveal" style="transition-delay: 0.2s;">
                    <img src="https://i.ibb.co/zVJcfsxp/valentine.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/10 group-hover:bg-black/40 flex items-center justify-center transition-all opacity-0 group-hover:opacity-100">
                        <span class="text-white text-[10px] tracking-[0.4em] uppercase border border-white px-6 py-2">Valentine</span>
                    </div>
                </div>

                <div class="overflow-hidden relative group h-[350px] reveal" style="transition-delay: 0.3s;">
                    <img src="https://i.ibb.co/1YPCtCV6/boy-s-day.jpg" class="img-zoom w-full h-full object-cover">
                    <div class="absolute inset-0 bg-black/10 group-hover:bg-black/40 flex items-center justify-center transition-all opacity-0 group-hover:opacity-100">
                        <span class="text-white text-[10px] tracking-[0.4em] uppercase border border-white px-6 py-2">Boy's Day</span>
                    </div>
                </div>
            </div>

        </div>
    </div>
</section>

    <section id="contact" class="py-32 px-6">
        <div class="max-w-4xl mx-auto text-center reveal">
            <h2 class="font-serif text-5xl italic mb-12">Connect with Meo</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-20 text-[11px] tracking-[0.2em] uppercase leading-loose opacity-80">
                <div>
                    <p class="font-bold mb-4">Address</p>
                    <p>Kiệt đối diện 68 Tố Hữu, Phường Xuân Phú, TP Huế</p>
                </div>
                <div>
                    <p class="font-bold mb-4">Contact</p>
                    <a href="tel:0941190148" class="hover:opacity-50">0941 190 148</a>
                </div>
                <div>
                    <p class="font-bold mb-4">Socials</p>
                    <div class="flex justify-center space-x-6">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                        <a href="#"><i class="fa-brands fa-tiktok"></i></a>
                    </div>
                </div>
            </div>
            <a href="tel:0941190148" class="px-16 py-6 bg-[#2f4f4f] text-white text-[11px] tracking-[0.4em] uppercase hover:bg-opacity-80 transition-all duration-500 shadow-xl">Gọi Tư Vấn Ngay</a>
        </div>
    </section>

    <footer class="py-12 border-t border-[#2f4f4f]/10 text-center">
        <p class="text-[9px] tracking-[0.3em] opacity-40 uppercase">© 2026 MEO FLOWERS STUDIO. ALL RIGHTS RESERVED.</p>
    </footer>

    <div class="fixed bottom-8 right-8 z-[100]">
        <a href="tel:0941190148" class="btn-pulse w-14 h-14 bg-[#2f4f4f] text-white rounded-full flex items-center justify-center text-xl shadow-2xl">
            <i class="fa-solid fa-phone"></i>
        </a>
    </div>

    <div id="productModal" class="fixed inset-0 z-[200] hidden flex items-center justify-center px-4">
        <div class="absolute inset-0 bg-black/60 backdrop-blur-sm" id="closeModalBg"></div>
        <div class="relative bg-[#fff5f7] w-full max-w-5xl max-h-[85vh] overflow-y-auto rounded-lg shadow-2xl p-8 md:p-12">
            <button id="closeModalBtn" class="absolute top-6 right-6 text-2xl hover:rotate-90 transition-transform duration-300">
                <i class="fa-solid fa-xmark"></i>
            </button>
            <div class="text-center mb-12">
                <h2 id="modalTitle" class="font-serif text-3xl italic mb-2">Sản phẩm</h2>
                <div class="w-12 h-[1px] bg-[#2f4f4f] mx-auto opacity-30"></div>
            </div>
            <div id="productGrid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                </div>
        </div>
    </div>

    <script>
        // 1. Data
        const eventData = {
            
            "valentine": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "wedding": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "opening": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],
            "boysday": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "womensday": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "graduation": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "noel": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "trungthu": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "blackwhite": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "mini": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "daily": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

             "signature": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

             "luxury": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

             "premium": [
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "},
                { price: "250.000", img: " "}
            ],

            "default": [
                { name: "Hoa Thiết Kế Riêng", price: "Liên hệ", img: "https://picsum.photos/400/500?random=10" }
            ]
        };

        // 2. Các phần tử DOM
        const modal = document.getElementById('productModal');
        const productGrid = document.getElementById('productGrid');
        const modalTitle = document.getElementById('modalTitle');
        const closeModalBtn = document.getElementById('closeModalBtn');
        const closeModalBg = document.getElementById('closeModalBg');

        // 3. Hàm hiển thị Modal (Đã sửa lỗi logic)
        function openModal(key, title) {
            const products = eventData[key] || eventData["default"];
            modalTitle.innerText = title;
            productGrid.innerHTML = '';

            products.forEach((item, index) => {
                const card = `
                    <div class="flower-card group bg-white p-4 shadow-sm border border-gray-100">
                        <div class="overflow-hidden mb-4 h-72 bg-gray-100">
                            <img src="${item.img}" class="img-zoom w-full h-full object-cover" alt="Product">
                        </div>
                        <div class="flex justify-between items-end mb-4">
                            <div>
                                <p class="text-[9px] tracking-widest uppercase opacity-60">Giá từ</p>
                                <p class="font-serif italic text-lg text-[#2f4f4f]">${item.price} VND</p>
                            </div>
                            <button onclick="toggleOrderForm(${index})" class="text-[9px] tracking-[0.2em] uppercase border-b border-[#2f4f4f] pb-1 hover:opacity-50 transition-all">
                                Đặt hàng ngay
                            </button>
                        </div>
                        <div id="form-${index}" class="hidden mt-4 pt-4 border-t border-dashed border-gray-200">
                            <div class="space-y-3">
                                <input type="text" id="name-${index}" placeholder="Họ Tên người nhận" class="w-full bg-transparent border-b border-gray-300 py-2 text-xs focus:outline-none focus:border-[#2f4f4f]">
                                <input type="text" id="phone-${index}" placeholder="Số điện thoại" class="w-full bg-transparent border-b border-gray-300 py-2 text-xs focus:outline-none focus:border-[#2f4f4f]">
                                <button onclick="sendToZalo('${item.price}', ${index})" class="w-full py-3 bg-[#2f4f4f] text-white text-[9px] tracking-[0.2em] uppercase mt-2">
                                    Gửi Tiệm Lên Đơn
                                </button>
                            </div>
                        </div>
                    </div>`;
                productGrid.innerHTML += card;
            });

            modal.classList.remove('hidden');
            document.body.style.overflow = 'hidden';
        }

        // 4. Các hàm hỗ trợ
        function closeModal() {
            modal.classList.add('hidden');
            document.body.style.overflow = '';
        }

        function toggleOrderForm(index) {
            const form = document.getElementById(`form-${index}`);
            form.classList.toggle('hidden');
        }

        function sendToZalo(price, index) {
            const name = document.getElementById(`name-${index}`).value;
            const phone = document.getElementById(`phone-${index}`).value;
            const message = `Chào Meo Flowers, mình muốn đặt mẫu hoa giá ${price}. Người nhận: ${name}, SĐT: ${phone}`;
            window.open(`https://zalo.me/0941190148?text=${encodeURIComponent(message)}`, '_blank');
        }

        // 5. Gắn sự kiện Click cho các danh mục (Quan trọng)
        document.querySelectorAll('[data-event]').forEach(button => {
            button.addEventListener('click', (e) => {
                e.preventDefault();
                const key = button.getAttribute('data-event');
                const title = button.innerText.split('\n')[0]; // Lấy tên hiển thị
                openModal(key, title);
            });
        });

        closeModalBtn.addEventListener('click', closeModal);
        closeModalBg.addEventListener('click', closeModal);

        // 6. Hiệu ứng cuộn (Scroll Reveal)
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");
            reveals.forEach(el => {
                var windowHeight = window.innerHeight;
                var elementTop = el.getBoundingClientRect().top;
                if (elementTop < windowHeight - 150) {
                    el.classList.add("active");
                }
            });
        }
        window.addEventListener("scroll", reveal);
        window.addEventListener("load", reveal);

        // Thêm vào phần JavaScript của bạn
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.querySelector('.md\\:flex'); // Chọn khối chứa link điều hướng

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('hidden');
            navLinks.classList.toggle('flex');
            navLinks.classList.toggle('flex-col');
            navLinks.classList.toggle('absolute');
            navLinks.classList.toggle('top-16');
            navLinks.classList.toggle('left-0');
            navLinks.classList.toggle('w-full');
            navLinks.classList.toggle('bg-white');
            navLinks.classList.toggle('p-6');
        });
    </script>
</body>
</html>
