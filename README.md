<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0" />
  <title>CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH | duongkienthanh.com</title>
  <meta name="description" content="CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH - Chuyên thiết kế kiến trúc, thi công phần thô, thi công hoàn thiện, xây nhà trọn gói và nội thất tại Đà Nẵng. Hotline: 0905.198.539." />
  <meta name="keywords" content="Dương Kiến Thành, thiết kế xây dựng Đà Nẵng, xây nhà trọn gói Đà Nẵng, thi công phần thô, thiết kế nội thất Đà Nẵng, duongkienthanh.com" />

  <!-- Open Graph / Thumbnail Logo khi chia sẻ đường dẫn trang web lên Zalo, Facebook -->
  <meta property="og:type" content="website" />
  <meta property="og:site_name" content="Dương Kiến Thành - Thiết Kế & Xây Dựng" />
  <meta property="og:title" content="CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH" />
  <meta property="og:description" content="Thiết kế Kiến trúc - Thi công phần thô - Hoàn thiện - Xây nhà trọn gói uy tín tại Đà Nẵng. Hotline: 0905.198.539." />
  <meta property="og:url" content="https://duongkienthanh.com/" />
  <meta property="og:image" content="https://duongkienthanh.com/wp-content/uploads/logo-duong-kien-thanh-og.png" />
  <meta property="og:image:width" content="1200" />
  <meta property="og:image:height" content="630" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH" />
  <meta name="twitter:description" content="Chuyên Thiết kế & Xây dựng trọn gói tại Đà Nẵng - Hotline: 0905.198.539" />
  <meta name="twitter:image" content="https://duongkienthanh.com/wp-content/uploads/logo-duong-kien-thanh-og.png" />

  <!-- Favicon Logo Công Ty -->
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='10' fill='%230F2A47'/%3E%3Cpath d='M12 46V26L32 13L52 26V46H43V30L32 23L21 30V46H12Z' fill='%23D49E35'/%3E%3Crect x='28' y='34' width='8' height='12' fill='%23FFFFFF'/%3E%3C/svg%3E" />

  <!-- Google Font Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              navy: '#0F2A47',
              navyDark: '#0A1E34',
              navyLight: '#193D66',
              gold: '#C8922A',
              goldLight: '#DDA83F',
              goldSoft: '#FBF5E8',
              slate: '#334155',
              bg: '#F7F8FA'
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif']
          }
        }
      }
    };
  </script>

  <style>
    /* Đảm bảo chuẩn khung hiển thị, tuyệt đối không tràn viền hay lệch sang phải */
    *, *::before, *::after {
      box-sizing: border-box;
    }

    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      max-width: 100%;
      overflow-x: hidden;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      font-size: 15px;
      line-height: 1.6;
      color: #1E293B;
      background-color: #FFFFFF;
      scroll-behavior: smooth;
      -webkit-font-smoothing: antialiased;
    }

    /* Container chuẩn Flatsome: 95% chiều ngang màn hình trên máy tính */
    .dkt-container {
      width: 100%;
      max-width: 100%;
      margin-left: auto;
      margin-right: auto;
      padding-left: 12px;
      padding-right: 12px;
    }

    @media (min-width: 640px) {
      .dkt-container {
        padding-left: 16px;
        padding-right: 16px;
      }
    }

    @media (min-width: 1024px) {
      .dkt-container {
        width: 95%;
        max-width: 95%;
        padding-left: 0;
        padding-right: 0;
      }
    }

    /* Đường gạch chân tiêu đề kiểu Flatsome */
    .section-title-bar {
      width: 56px;
      height: 3px;
      background-color: #C8922A;
      margin-top: 10px;
      border-radius: 9999px;
    }

    /* Hiệu ứng trượt mượt cho 2 banner bằng kích thước nhau */
    .banner-track {
      display: grid;
      grid-template-columns: 1fr;
      grid-template-rows: 1fr;
      width: 100%;
      position: relative;
      overflow: hidden;
    }

    .banner-slide {
      grid-area: 1 / 1 / 2 / 2;
      width: 100%;
      transition: opacity 0.7s ease-in-out, transform 0.7s ease-in-out;
    }

    .banner-slide.is-active {
      opacity: 1;
      z-index: 2;
      pointer-events: auto;
      transform: scale(1);
    }

    .banner-slide.is-inactive {
      opacity: 0;
      z-index: 1;
      pointer-events: none;
      transform: scale(1.015);
    }

    /* Dropdown menu gọn đẹp kiểu Flatsome */
    .nav-item-group:hover .nav-dropdown {
      opacity: 1;
      visibility: visible;
      transform: translateY(0);
    }

    .nav-dropdown {
      opacity: 0;
      visibility: hidden;
      transform: translateY(6px);
      transition: all 0.2s ease;
    }

    /* Thanh cuộn ẩn gọn cho tab danh mục trên điện thoại */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    /* Hiệu ứng rung nhẹ cho nút Hotline nổi */
    @keyframes phonePulse {
      0% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.45); }
      70% { box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
      100% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
    }
    .hotline-pulse {
      animation: phonePulse 2s infinite;
    }
  </style>
</head>

<body class="bg-white text-slate-800">

  <!-- ==================== TOP BAR (PHONG CÁCH FLATSOME - KHÔNG CÓ TÙY CHỈNH UXBUILDER) ==================== -->
  <div class="w-full bg-brand-navy text-white text-xs border-b border-brand-navyLight">
    <div class="dkt-container py-2 flex flex-wrap items-center justify-between gap-2">
      <div class="flex flex-wrap items-center gap-x-4 gap-y-1">
        <a href="tel:0905198539" class="inline-flex items-center gap-1.5 hover:text-brand-goldLight transition-colors whitespace-nowrap font-medium">
          <svg class="w-3.5 h-3.5 text-brand-goldLight shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
          </svg>
          <span>Hotline: 0905.198.539</span>
        </a>
        <span class="hidden sm:inline text-white/30">|</span>
        <span class="hidden sm:inline-flex items-center gap-1.5 text-slate-200 truncate">
          <svg class="w-3.5 h-3.5 text-brand-goldLight shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
          </svg>
          <span>KĐT Hòa Quý, P. Ngũ Hành Sơn, TP. Đà Nẵng</span>
        </span>
      </div>
      <div class="hidden md:flex items-center gap-3 text-slate-200">
        <span class="whitespace-nowrap">Website: <strong class="text-brand-goldLight font-semibold">duongkienthanh.com</strong></span>
        <span class="text-white/30">|</span>
        <span class="whitespace-nowrap">MST: 0402171855</span>
      </div>
    </div>
  </div>

  <!-- ==================== HEADER CHÍNH (LOGO GỌN NHỎ, MENU 1 HÀNG KHÔNG XUỐNG DÒNG, KHÔNG CÓ NÚT GỌI NGAY) ==================== -->
  <header class="w-full bg-white sticky top-0 z-40 shadow-sm border-b border-slate-200">
    <div class="dkt-container h-16 lg:h-[68px] flex items-center justify-between gap-3">

      <!-- Logo Công Ty Thiết Kế Chuyên Nghiệp, Gọn Nhỏ -->
      <a href="#trang-chu" class="flex items-center gap-2.5 shrink-0 group" aria-label="Dương Kiến Thành Trang Chủ">
        <div class="w-9 h-9 sm:w-10 sm:h-10 rounded-lg bg-brand-navy flex items-center justify-center shadow-sm shrink-0 border border-brand-gold/40">
          <!-- Biểu tượng kiến trúc DKT gọn sắc nét -->
          <svg class="w-6 h-6 sm:w-7 sm:h-7" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M6 36V19.5L24 8L42 19.5V36H35.5V22.8L24 15.6L12.5 22.8V36H6Z" fill="#D49E35"/>
            <path d="M17 36V25.5L24 21L31 25.5V36H26.5V28.5H21.5V36H17Z" fill="#FFFFFF"/>
            <rect x="6" y="38.5" width="36" height="2.5" rx="1.25" fill="#D49E35"/>
          </svg>
        </div>
        <div class="flex flex-col leading-tight">
          <span class="text-[13px] sm:text-[15px] font-extrabold tracking-tight text-brand-navy whitespace-nowrap group-hover:text-brand-gold transition-colors">
            DƯƠNG KIẾN THÀNH
          </span>
          <span class="text-[9px] sm:text-[10px] font-semibold tracking-[0.12em] text-brand-gold uppercase whitespace-nowrap">
            THIẾT KẾ &amp; XÂY DỰNG
          </span>
        </div>
      </a>

      <!-- Menu Máy Tính: Viết liền trên 1 hàng, chữ nhỏ gọn, tuyệt đối không xuống dòng tên danh mục -->
      <nav class="hidden lg:flex items-center justify-end flex-nowrap gap-0.5 xl:gap-1.5" aria-label="Menu chính">
        <a href="#trang-chu" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-brand-navy hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Trang chủ
        </a>
        <a href="#gioi-thieu" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Giới thiệu
        </a>

        <!-- Dropdown: Công trình thực tế (theo web mẫu Tín Trường Thịnh) -->
        <div class="relative nav-item-group">
          <a href="#cong-trinh-thuc-te" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap inline-flex items-center gap-1 rounded-md">
            <span>Công trình thực tế</span>
            <svg class="w-3 h-3 opacity-70 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M19 9l-7 7-7-7"/></svg>
          </a>
          <div class="nav-dropdown absolute left-0 top-full pt-1 w-56 z-50">
            <div class="bg-white rounded-lg shadow-xl border border-slate-100 py-1.5">
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('khach-san-can-ho')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Khách sạn – Căn hộ – Phòng trọ</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('biet-thu')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Biệt thự</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('nha-pho')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Nhà phố</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('van-phong')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Văn phòng</a>
            </div>
          </div>
        </div>

        <!-- Dropdown: Lĩnh vực hoạt động -->
        <div class="relative nav-item-group">
          <a href="#linh-vuc" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap inline-flex items-center gap-1 rounded-md">
            <span>Lĩnh vực hoạt động</span>
            <svg class="w-3 h-3 opacity-70 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M19 9l-7 7-7-7"/></svg>
          </a>
          <div class="nav-dropdown absolute left-0 top-full pt-1 w-56 z-50">
            <div class="bg-white rounded-lg shadow-xl border border-slate-100 py-1.5">
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('thiet-ke-kien-truc')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Thiết kế Kiến trúc – Nội thất</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-phan-tho')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Thi công phần thô</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-hoan-thien')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Thi công hoàn thiện</a>
              <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-noi-that')" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Thi công nội thất</a>
            </div>
          </div>
        </div>

        <!-- Dropdown: Báo giá -->
        <div class="relative nav-item-group">
          <a href="#bao-gia" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap inline-flex items-center gap-1 rounded-md">
            <span>Báo giá</span>
            <svg class="w-3 h-3 opacity-70 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M19 9l-7 7-7-7"/></svg>
          </a>
          <div class="nav-dropdown absolute left-0 top-full pt-1 w-56 z-50">
            <div class="bg-white rounded-lg shadow-xl border border-slate-100 py-1.5">
              <a href="#bao-gia" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Báo giá thiết kế kiến trúc</a>
              <a href="#bao-gia" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Báo giá thi công phần thô</a>
              <a href="#bao-gia" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Báo giá thi công hoàn thiện</a>
              <a href="#bao-gia" class="block px-4 py-2 text-[12.5px] font-medium text-slate-700 hover:bg-brand-goldSoft hover:text-brand-navy whitespace-nowrap">Báo giá thi công trọn gói</a>
            </div>
          </div>
        </div>

        <a href="#du-an-da-nang" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Dự án Đà Nẵng
        </a>
        <a href="#doi-tac" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Đối tác
        </a>
        <a href="#tin-tuc" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Tin tức
        </a>
        <a href="#lien-he" class="px-2 xl:px-2.5 py-2 text-[12px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-gold transition-colors whitespace-nowrap rounded-md">
          Liên hệ
        </a>
      </nav>

      <!-- Nút Mở Menu Mobile (Không đặt nút Gọi ngay trên Header) -->
      <button id="mobileMenuBtn" type="button" onclick="toggleMobileMenu()" aria-label="Mở menu điều hướng" class="lg:hidden p-2.5 rounded-lg text-brand-navy hover:bg-slate-100 focus:outline-none">
        <svg id="menuIconOpen" class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg id="menuIconClose" class="w-6 h-6 hidden" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>

    <!-- Menu Điều Hướng Điện Thoại -->
    <div id="mobileMenu" class="lg:hidden hidden bg-white border-t border-slate-200 shadow-lg">
      <div class="dkt-container py-3 flex flex-col divide-y divide-slate-100">
        <a href="#trang-chu" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-brand-navy hover:text-brand-gold">Trang chủ</a>
        <a href="#gioi-thieu" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Giới thiệu</a>
        <a href="#linh-vuc" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Lĩnh vực hoạt động</a>
        <a href="#cong-trinh-thuc-te" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Công trình thực tế</a>
        <a href="#du-an-da-nang" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Dự án Đà Nẵng</a>
        <a href="#bao-gia" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Báo giá thiết kế &amp; thi công</a>
        <a href="#doi-tac" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Đối tác</a>
        <a href="#tin-tuc" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Tin tức</a>
        <a href="#lien-he" onclick="closeMobileMenu()" class="py-2.5 px-2 text-sm font-semibold text-slate-700 hover:text-brand-gold">Liên hệ &amp; Báo giá</a>
      </div>
    </div>
  </header>

  <main id="trang-chu" class="w-full overflow-x-hidden">

    <!-- ==================== 2 ẢNH BANNER TỰ TRƯỢT KÍCH THƯỚC BẰNG NHAU, CHỮ NẰM TRỌN TRONG KHUNG CÁCH XA VIỀN ==================== -->
    <section class="w-full bg-brand-navyDark">
      <div class="dkt-container py-0 lg:py-4">
        <div class="relative w-full rounded-none lg:rounded-xl overflow-hidden shadow-md bg-brand-navyDark" id="heroSlider">
          <div class="banner-track">

            <!-- Banner 1 -->
            <div class="banner-slide is-active relative flex items-center" data-slide="0">
              <img
                src="https://drive.google.com/thumbnail?id=1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR&sz=w1600"
                data-fallback="https://lh3.googleusercontent.com/d/1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR"
                alt="Thiết kế và thi công xây dựng trọn gói Dương Kiến Thành"
                class="absolute inset-0 w-full h-full object-cover object-center"
                onerror="handleDriveImageError(this, 'Dương Kiến Thành - Xây Dựng Trọn Gói')"
              />
              <!-- Lớp phủ gradient giúp chữ sắc nét hoàn hảo -->
              <div class="absolute inset-0 bg-gradient-to-r from-brand-navyDark/92 via-brand-navy/80 to-brand-navyDark/55"></div>

              <!-- Vùng nội dung cách xa viền ảnh banner an toàn trên cả điện thoại và máy tính -->
              <div class="relative z-10 w-full px-10 py-12 sm:px-16 sm:py-16 md:px-20 md:py-20 lg:px-24 lg:py-24">
                <div class="max-w-2xl">
                  <p class="text-[11px] sm:text-xs font-bold uppercase tracking-[0.18em] text-brand-goldLight mb-2.5">
                    CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH
                  </p>
                  <h1 class="text-xl sm:text-3xl md:text-4xl lg:text-[40px] font-extrabold text-white leading-snug mb-3.5">
                    KIẾN TẠO KHÔNG GIAN SỐNG BỀN VỮNG TẠI ĐÀ NẴNG
                  </h1>
                  <p class="text-xs sm:text-sm md:text-base text-slate-200 leading-relaxed mb-6">
                    Chuyên Thiết kế Kiến trúc – Thi công phần thô – Hoàn thiện nội thất và Xây nhà trọn gói. Cam kết đúng tiến độ, chuẩn kỹ thuật và tối ưu chi phí cho mọi công trình.
                  </p>
                  <div class="flex flex-wrap items-center gap-3">
                    <a href="#lien-he" class="px-5 py-2.5 rounded-lg bg-brand-gold hover:bg-brand-goldLight text-white font-semibold text-xs sm:text-sm transition-colors shadow">
                      Nhận Báo Giá Miễn Phí
                    </a>
                    <a href="#cong-trinh-thuc-te" class="px-5 py-2.5 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/40 font-semibold text-xs sm:text-sm transition-colors">
                      Xem Công Trình Thực Tế
                    </a>
                  </div>
                </div>
              </div>
            </div>

            <!-- Banner 2 (Cùng kích thước 100% với Banner 1 nhờ CSS Grid Stack) -->
            <div class="banner-slide is-inactive relative flex items-center" data-slide="1">
              <img
                src="https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w1600"
                data-fallback="https://lh3.googleusercontent.com/d/157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT"
                alt="Thi công nhà phố, biệt thự, căn hộ, khách sạn tại Đà Nẵng"
                class="absolute inset-0 w-full h-full object-cover object-center"
                onerror="handleDriveImageError(this, 'Dự Án Thực Tế Tại Đà Nẵng')"
              />
              <div class="absolute inset-0 bg-gradient-to-r from-brand-navyDark/92 via-brand-navy/80 to-brand-navyDark/55"></div>

              <!-- Vùng nội dung cách xa viền ảnh banner an toàn trên cả điện thoại và máy tính -->
              <div class="relative z-10 w-full px-10 py-12 sm:px-16 sm:py-16 md:px-20 md:py-20 lg:px-24 lg:py-24">
                <div class="max-w-2xl">
                  <p class="text-[11px] sm:text-xs font-bold uppercase tracking-[0.18em] text-brand-goldLight mb-2.5">
                    GIẢI PHÁP XÂY DỰNG CHÌA KHÓA TRAO TAY
                  </p>
                  <h2 class="text-xl sm:text-3xl md:text-4xl lg:text-[40px] font-extrabold text-white leading-snug mb-3.5">
                    NHÀ Ở GIA ĐÌNH – TIÊU CHUẨN CÔNG TRÌNH CHUYÊN NGHIỆP
                  </h2>
                  <p class="text-xs sm:text-sm md:text-base text-slate-200 leading-relaxed mb-6">
                    Đội ngũ kỹ sư, kiến trúc sư giàu kinh nghiệm trực tiếp giám sát thi công Nhà phố, Biệt thự, Khách sạn, Căn hộ và Văn phòng tại Hòa Quý, Hòa Xuân và khắp TP. Đà Nẵng.
                  </p>
                  <div class="flex flex-wrap items-center gap-3">
                    <a href="#du-an-da-nang" class="px-5 py-2.5 rounded-lg bg-brand-gold hover:bg-brand-goldLight text-white font-semibold text-xs sm:text-sm transition-colors shadow">
                      Khám Phá Dự Án Đà Nẵng
                    </a>
                    <a href="tel:0905198539" class="px-5 py-2.5 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/40 font-semibold text-xs sm:text-sm transition-colors">
                      Tư Vấn: 0905.198.539
                    </a>
                  </div>
                </div>
              </div>
            </div>

          </div>

          <!-- Nút chuyển slide trái / phải đặt sát mép ngoài, không đè lên chữ -->
          <button type="button" onclick="prevSlide()" aria-label="Banner trước" class="absolute left-2 sm:left-3 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-brand-gold text-white flex items-center justify-center transition-colors">
            <svg class="w-4 h-4 sm:w-5 sm:h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M15 19l-7-7 7-7"/></svg>
          </button>
          <button type="button" onclick="nextSlide()" aria-label="Banner tiếp theo" class="absolute right-2 sm:right-3 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-brand-gold text-white flex items-center justify-center transition-colors">
            <svg class="w-4 h-4 sm:w-5 sm:h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M9 5l7 7-7 7"/></svg>
          </button>

          <!-- Chấm chỉ báo 2 banner -->
          <div class="absolute bottom-3.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
            <button type="button" onclick="goToSlide(0)" id="dot-0" aria-label="Banner 1" class="w-6 h-2 rounded-full bg-brand-gold transition-all"></button>
            <button type="button" onclick="goToSlide(1)" id="dot-1" aria-label="Banner 2" class="w-2.5 h-2 rounded-full bg-white/50 hover:bg-white transition-all"></button>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== DỊCH VỤ TIÊU BIỂU (GIỐNG WEB MẪU TÍN TRƯỜNG THỊNH - PHONG CÁCH FLATSOME ĐƠN GIẢN) ==================== -->
    <section id="linh-vuc" class="py-10 sm:py-14 bg-white">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-8 sm:mb-10">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Lĩnh Vực Hoạt Động Tiêu Biểu
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Cung cấp giải pháp toàn diện từ khâu lên ý tưởng kiến trúc đến thi công hoàn thiện và bàn giao công trình.
          </p>
        </div>

        <div class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
          <!-- Dịch vụ 1 -->
          <a href="#cong-trinh-thuc-te" onclick="filterProducts('thiet-ke-kien-truc')" class="group bg-brand-bg hover:bg-white rounded-xl p-4 sm:p-6 border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all text-center flex flex-col items-center">
            <div class="w-12 h-12 rounded-xl bg-brand-navy text-brand-goldLight flex items-center justify-center mb-3.5 group-hover:bg-brand-gold group-hover:text-white transition-colors">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
            </div>
            <h3 class="text-sm sm:text-base font-bold text-brand-navy group-hover:text-brand-gold transition-colors mb-1.5">
              Thiết Kế Kiến Trúc – Nội Thất
            </h3>
            <p class="text-xs text-slate-600 leading-relaxed">
              Thiết kế mặt tiền, công năng khoa học, hồ sơ bản vẽ 2D &amp; phối cảnh 3D chuẩn phong thủy.
            </p>
          </a>

          <!-- Dịch vụ 2 -->
          <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-phan-tho')" class="group bg-brand-bg hover:bg-white rounded-xl p-4 sm:p-6 border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all text-center flex flex-col items-center">
            <div class="w-12 h-12 rounded-xl bg-brand-navy text-brand-goldLight flex items-center justify-center mb-3.5 group-hover:bg-brand-gold group-hover:text-white transition-colors">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"/></svg>
            </div>
            <h3 class="text-sm sm:text-base font-bold text-brand-navy group-hover:text-brand-gold transition-colors mb-1.5">
              Thi Công Phần Thô
            </h3>
            <p class="text-xs text-slate-600 leading-relaxed">
              Thi công kết cấu móng, khung cột, dầm sàn bê tông cốt thép vững chắc, vật tư đúng cam kết.
            </p>
          </a>

          <!-- Dịch vụ 3 -->
          <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-hoan-thien')" class="group bg-brand-bg hover:bg-white rounded-xl p-4 sm:p-6 border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all text-center flex flex-col items-center">
            <div class="w-12 h-12 rounded-xl bg-brand-navy text-brand-goldLight flex items-center justify-center mb-3.5 group-hover:bg-brand-gold group-hover:text-white transition-colors">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"/></svg>
            </div>
            <h3 class="text-sm sm:text-base font-bold text-brand-navy group-hover:text-brand-gold transition-colors mb-1.5">
              Thi Công Hoàn Thiện Trọn Gói
            </h3>
            <p class="text-xs text-slate-600 leading-relaxed">
              Ốp lát, sơn nước, chống thấm, điện nước M&amp;E tỉ mỉ, sắc nét, bàn giao chìa khóa trao tay.
            </p>
          </a>

          <!-- Dịch vụ 4 -->
          <a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-noi-that')" class="group bg-brand-bg hover:bg-white rounded-xl p-4 sm:p-6 border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all text-center flex flex-col items-center">
            <div class="w-12 h-12 rounded-xl bg-brand-navy text-brand-goldLight flex items-center justify-center mb-3.5 group-hover:bg-brand-gold group-hover:text-white transition-colors">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z"/></svg>
            </div>
            <h3 class="text-sm sm:text-base font-bold text-brand-navy group-hover:text-brand-gold transition-colors mb-1.5">
              Thi Công Nội Thất
            </h3>
            <p class="text-xs text-slate-600 leading-relaxed">
              Sản xuất và lắp đặt nội thất nhà phố, biệt thự, căn hộ, văn phòng chuẩn bản vẽ 3D.
            </p>
          </a>
        </div>
      </div>
    </section>

    <!-- ==================== GIỚI THIỆU & THẾ MẠNH CỦA CHÚNG TÔI (THEO BỐ CỤC WEB MẪU) ==================== -->
    <section id="gioi-thieu" class="py-10 sm:py-14 bg-brand-bg border-y border-slate-200/80">
      <div class="dkt-container">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center mb-10 sm:mb-12">
          <!-- Cột nội dung giới thiệu -->
          <div class="lg:col-span-6">
            <p class="text-xs font-bold uppercase tracking-widest text-brand-gold mb-2">VỀ CHÚNG TÔI</p>
            <h2 class="text-xl sm:text-2xl lg:text-[28px] font-extrabold text-brand-navy leading-snug">
              CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH
            </h2>
            <div class="section-title-bar mb-5"></div>
            <p class="text-sm text-slate-600 leading-relaxed mb-4">
              <strong>DƯƠNG KIẾN THÀNH</strong> chuyên Thiết kế – Xây dựng – Nội thất các công trình Nhà phố, Biệt thự, Khách sạn, Căn hộ cho thuê và Văn phòng tại khu vực Đà Nẵng và Quảng Nam.
            </p>
            <p class="text-sm text-slate-600 leading-relaxed mb-5">
              Với phương châm <strong>“An Toàn – Chất Lượng – Tiến Độ – Tận Tâm”</strong>, chúng tôi đặt chữ TÍN lên hàng đầu trong từng hạng mục thi công thực tế, đảm bảo công trình đạt chuẩn kỹ thuật, thẩm mỹ cao và tối ưu ngân sách cho chủ đầu tư.
            </p>
            <div class="grid grid-cols-3 gap-3 pt-2">
              <div class="bg-white rounded-lg p-3.5 text-center border border-slate-200">
                <div class="text-xl sm:text-2xl font-extrabold text-brand-navy">100%</div>
                <div class="text-[11px] sm:text-xs text-slate-600 mt-0.5">Đúng tiến độ</div>
              </div>
              <div class="bg-white rounded-lg p-3.5 text-center border border-slate-200">
                <div class="text-xl sm:text-2xl font-extrabold text-brand-gold">5 Năm</div>
                <div class="text-[11px] sm:text-xs text-slate-600 mt-0.5">Bảo hành kết cấu</div>
              </div>
              <div class="bg-white rounded-lg p-3.5 text-center border border-slate-200">
                <div class="text-xl sm:text-2xl font-extrabold text-brand-navy">24/7</div>
                <div class="text-[11px] sm:text-xs text-slate-600 mt-0.5">Tư vấn tận tâm</div>
              </div>
            </div>
          </div>

          <!-- Cột ảnh thi công thực tế (không có nhãn dán) -->
          <div class="lg:col-span-6">
            <div class="grid grid-cols-2 gap-3 sm:gap-4">
              <div class="rounded-xl overflow-hidden shadow-sm border border-slate-200 bg-white aspect-[4/3]">
                <img
                  src="https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w1000"
                  data-fallback="https://lh3.googleusercontent.com/d/13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz"
                  alt="Thi công thực tế Dương Kiến Thành"
                  class="w-full h-full object-cover"
                  onerror="handleDriveImageError(this, 'Thi Công Thực Tế')"
                />
              </div>
              <div class="rounded-xl overflow-hidden shadow-sm border border-slate-200 bg-white aspect-[4/3]">
                <img
                  src="https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w1000"
                  data-fallback="https://lh3.googleusercontent.com/d/1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv"
                  alt="Đội ngũ thi công xây dựng tại Đà Nẵng"
                  class="w-full h-full object-cover"
                  onerror="handleDriveImageError(this, 'Xây Dựng Đà Nẵng')"
                />
              </div>
            </div>
          </div>
        </div>

        <!-- 6 Thế mạnh của chúng tôi -->
        <div class="pt-4">
          <h3 class="text-lg sm:text-xl font-bold text-brand-navy text-center mb-6 uppercase tracking-wide">
            Thế Mạnh Của Dương Kiến Thành
          </h3>
          <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">01</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Đội ngũ KTS &amp; kỹ sư chuyên nghiệp</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Kiến trúc sư sáng tạo cùng đội ngũ kỹ sư, thợ xây lành nghề nhiều năm kinh nghiệm thực chiến.</p>
              </div>
            </div>
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">02</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Cập nhật xu hướng thiết kế hiện đại</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Liên tục áp dụng giải pháp kiến trúc thông thoáng, vật liệu mới và công nghệ thi công tiên tiến.</p>
              </div>
            </div>
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">03</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Giám sát tiến độ chuẩn xác</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Báo cáo tiến độ công trình định kỳ giúp gia chủ dễ dàng theo dõi minh bạch mọi công đoạn.</p>
              </div>
            </div>
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">04</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Bảo hành công trình lâu dài</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Chế độ hậu mãi tận tâm, xử lý nhanh chóng khi khách hàng cần hỗ trợ sau bàn giao.</p>
              </div>
            </div>
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">05</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Chi phí minh bạch, không phát sinh</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Dự toán chi tiết rõ ràng từng hạng mục vật tư, cân đối ngân sách hợp lý nhất cho chủ đầu tư.</p>
              </div>
            </div>
            <div class="bg-white rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
              <div class="w-10 h-10 rounded-lg bg-brand-goldSoft text-brand-gold flex items-center justify-center shrink-0 font-bold">06</div>
              <div>
                <h4 class="text-sm font-bold text-brand-navy mb-1">Hỗ trợ tư vấn miễn phí 24/7</h4>
                <p class="text-xs text-slate-600 leading-relaxed">Tư vấn pháp lý xin phép xây dựng, thiết kế sơ bộ và báo giá nhanh qua Hotline/Zalo 0905.198.539.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== DANH MỤC SẢN PHẨM & CÔNG TRÌNH THỰC TẾ (9 ẢNH GOOGLE DRIVE THI CÔNG THỰC TẾ) ==================== -->
    <section id="cong-trinh-thuc-te" class="py-10 sm:py-14 bg-white">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-6">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Công Trình Thực Tế &amp; Danh Mục Sản Phẩm
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Hình ảnh thi công thực tế các hạng mục nhà phố, biệt thự, căn hộ, khách sạn và văn phòng do Dương Kiến Thành trực tiếp triển khai.
          </p>
        </div>

        <!-- Thanh Danh Mục Trang Chủ: Chữ nhỏ gọn, viết liền không xuống dòng tên danh mục, đẹp trên cả máy tính và điện thoại -->
        <div class="mb-7">
          <div id="categoryTabs" class="flex flex-nowrap lg:flex-wrap overflow-x-auto lg:overflow-visible no-scrollbar justify-start lg:justify-center gap-2 pb-1">
            <button type="button" onclick="filterProducts('all')" data-cat="all" class="cat-tab active-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-brand-navy text-white border-brand-navy">
              Tất cả
            </button>
            <button type="button" onclick="filterProducts('nha-pho')" data-cat="nha-pho" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Nhà phố
            </button>
            <button type="button" onclick="filterProducts('biet-thu')" data-cat="biet-thu" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Biệt thự
            </button>
            <button type="button" onclick="filterProducts('khach-san-can-ho')" data-cat="khach-san-can-ho" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Khách sạn – Căn hộ
            </button>
            <button type="button" onclick="filterProducts('van-phong')" data-cat="van-phong" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Văn phòng
            </button>
            <button type="button" onclick="filterProducts('thiet-ke-kien-truc')" data-cat="thiet-ke-kien-truc" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Thiết kế kiến trúc
            </button>
            <button type="button" onclick="filterProducts('thi-cong-phan-tho')" data-cat="thi-cong-phan-tho" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Thi công phần thô
            </button>
            <button type="button" onclick="filterProducts('thi-cong-hoan-thien')" data-cat="thi-cong-hoan-thien" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Thi công hoàn thiện
            </button>
            <button type="button" onclick="filterProducts('thi-cong-noi-that')" data-cat="thi-cong-noi-that" class="cat-tab px-3.5 py-2 rounded-lg text-[12px] sm:text-[12.5px] font-semibold whitespace-nowrap border transition-all bg-white text-slate-700 border-slate-200 hover:border-brand-gold hover:text-brand-navy">
              Thi công nội thất
            </button>
          </div>
        </div>

        <!-- Lưới sản phẩm: 2 cột trên điện thoại, 3 cột trên máy tính bảng/desktop, KHÔNG có nhãn dán trên ảnh, tên sản phẩm hiển thị đầy đủ không thiếu chữ -->
        <div id="productGrid" class="grid grid-cols-2 md:grid-cols-3 gap-3 sm:gap-5">
          <!-- Render tự động bằng JS từ danh sách 9 ảnh thực tế Google Drive -->
        </div>
      </div>
    </section>

    <!-- ==================== DỰ ÁN TIÊU BIỂU TẠI ĐÀ NẴNG (10 ẢNH GOOGLE DRIVE DỰ ÁN ĐÀ NẴNG) ==================== -->
    <section id="du-an-da-nang" class="py-10 sm:py-14 bg-brand-bg border-y border-slate-200/80">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-8">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Các Dự Án Tiêu Biểu Tại Đà Nẵng
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Tổng hợp các công trình xây dựng và thiết kế thực tế tại Ngũ Hành Sơn, Hòa Quý, Hòa Xuân, Sơn Trà, Hải Châu và Cẩm Lệ.
          </p>
        </div>

        <!-- 2 cột trên điện thoại, 3 cột tablet, 5 cột trên máy tính (2 hàng 5 ảnh cực gọn đẹp), không nhãn dán -->
        <div id="danangProjectGrid" class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 gap-3 sm:gap-4">
          <!-- Render tự động bằng JS từ danh sách 10 ảnh dự án Đà Nẵng -->
        </div>
      </div>
    </section>

    <!-- ==================== BÁO GIÁ DỊCH VỤ (THEO DANH MỤC WEB MẪU TÍN TRƯỜNG THỊNH) ==================== -->
    <section id="bao-gia" class="py-10 sm:py-14 bg-white">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-8">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Báo Giá Thiết Kế &amp; Thi Công Tham Khảo
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Đơn giá xây dựng tại Đà Nẵng rõ ràng, cạnh tranh. Liên hệ ngay để nhận bảng dự toán chi tiết theo diện tích đất của bạn.
          </p>
        </div>

        <div class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
          <!-- Gói 1 -->
          <div class="bg-brand-bg rounded-xl p-4 sm:p-6 border border-slate-200 flex flex-col justify-between">
            <div>
              <h3 class="text-sm sm:text-base font-bold text-brand-navy mb-2">Báo Giá Thiết Kế Kiến Trúc</h3>
              <div class="text-base sm:text-xl font-extrabold text-brand-gold mb-3">Từ 150.000đ / m²</div>
              <ul class="text-xs text-slate-600 space-y-1.5 mb-5">
                <li>• Bản vẽ thiết kế 2D &amp; 3D mặt tiền</li>
                <li>• Hồ sơ kết cấu, điện nước đầy đủ</li>
                <li>• Hỗ trợ xin giấy phép xây dựng</li>
              </ul>
            </div>
            <a href="#lien-he" onclick="preselectQuote('Thiết kế Kiến trúc')" class="w-full py-2 px-3 rounded-lg bg-brand-navy hover:bg-brand-gold text-white text-xs font-semibold text-center transition-colors">
              Nhận Báo Giá
            </a>
          </div>

          <!-- Gói 2 -->
          <div class="bg-brand-bg rounded-xl p-4 sm:p-6 border border-slate-200 flex flex-col justify-between">
            <div>
              <h3 class="text-sm sm:text-base font-bold text-brand-navy mb-2">Báo Giá Thi Công Phần Thô</h3>
              <div class="text-base sm:text-xl font-extrabold text-brand-gold mb-3">Từ 3.500.000đ / m²</div>
              <ul class="text-xs text-slate-600 space-y-1.5 mb-5">
                <li>• Vật tư phần thô chính hãng</li>
                <li>• Nhân công phần thô &amp; hoàn thiện</li>
                <li>• Kỹ sư giám sát trực tiếp 100%</li>
              </ul>
            </div>
            <a href="#lien-he" onclick="preselectQuote('Thi công phần thô')" class="w-full py-2 px-3 rounded-lg bg-brand-navy hover:bg-brand-gold text-white text-xs font-semibold text-center transition-colors">
              Nhận Báo Giá
            </a>
          </div>

          <!-- Gói 3 -->
          <div class="bg-brand-bg rounded-xl p-4 sm:p-6 border border-slate-200 flex flex-col justify-between">
            <div>
              <h3 class="text-sm sm:text-base font-bold text-brand-navy mb-2">Báo Giá Thi Công Hoàn Thiện</h3>
              <div class="text-base sm:text-xl font-extrabold text-brand-gold mb-3">Từ 2.400.000đ / m²</div>
              <ul class="text-xs text-slate-600 space-y-1.5 mb-5">
                <li>• Sơn nước, gạch ốp lát, thiết bị vệ sinh</li>
                <li>• Cửa nhôm kính, cầu thang, trần thạch cao</li>
                <li>• Chủng loại vật tư theo yêu cầu</li>
              </ul>
            </div>
            <a href="#lien-he" onclick="preselectQuote('Thi công hoàn thiện')" class="w-full py-2 px-3 rounded-lg bg-brand-navy hover:bg-brand-gold text-white text-xs font-semibold text-center transition-colors">
              Nhận Báo Giá
            </a>
          </div>

          <!-- Gói 4 -->
          <div class="bg-brand-navy rounded-xl p-4 sm:p-6 border border-brand-navy text-white flex flex-col justify-between shadow-sm">
            <div>
              <h3 class="text-sm sm:text-base font-bold text-white mb-2">Báo Giá Thi Công Trọn Gói</h3>
              <div class="text-base sm:text-xl font-extrabold text-brand-goldLight mb-3">Từ 5.800.000đ / m²</div>
              <ul class="text-xs text-slate-200 space-y-1.5 mb-5">
                <li>• Miễn phí thiết kế khi ký trọn gói</li>
                <li>• Bao trọn vật tư thô &amp; hoàn thiện</li>
                <li>• Bảo hành kết cấu dài hạn 5 năm</li>
              </ul>
            </div>
            <a href="#lien-he" onclick="preselectQuote('Xây nhà trọn gói')" class="w-full py-2 px-3 rounded-lg bg-brand-gold hover:bg-brand-goldLight text-white text-xs font-semibold text-center transition-colors">
              Nhận Báo Giá
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== DANH MỤC CÁC ĐỐI TÁC ==================== -->
    <section id="doi-tac" class="py-10 sm:py-12 bg-brand-bg border-y border-slate-200/80">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-7">
          <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-wide">
            Đối Tác &amp; Nhà Cung Cấp Vật Tư
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-2.5 text-xs sm:text-sm text-slate-600">
            Hợp tác cùng các thương hiệu vật liệu xây dựng hàng đầu để đảm bảo chất lượng bền vững cho mọi công trình.
          </p>
        </div>

        <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-8 gap-3">
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">HÒA PHÁT</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Thép xây dựng</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">SÔNG GIANH</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Xi măng cao cấp</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">DULUX</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Sơn trang trí</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">JOTUN</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Sơn nội ngoại thất</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">XINGFA</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Nhôm kính cao cấp</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">AN CƯỜNG</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Gỗ nội thất</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">PANASONIC</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Thiết bị điện</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 px-3 py-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
            <span class="text-sm font-extrabold text-brand-navy tracking-tight">ĐỒNG TÂM</span>
            <span class="text-[10px] text-slate-500 mt-0.5">Gạch ốp lát</span>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== DANH MỤC CÁC BÀI VIẾT TRANG CHỦ ==================== -->
    <section id="tin-tuc" class="py-10 sm:py-14 bg-white">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-8">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Tin Tức &amp; Cẩm Nang Xây Dựng
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Chia sẻ kiến thức kỹ thuật thi công, xu hướng thiết kế nhà đẹp và kinh nghiệm xây dựng nhà tiết kiệm chi phí.
          </p>
        </div>

        <div id="articlesGrid" class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
          <!-- Render tự động bằng JS -->
        </div>
      </div>
    </section>

    <!-- ==================== FORM YÊU CẦU BÁO GIÁ + GOOGLE MAP + FACEBOOK NGAY TRANG CHỦ ==================== -->
    <section id="lien-he" class="py-10 sm:py-14 bg-brand-bg border-t border-slate-200">
      <div class="dkt-container">
        <div class="text-center max-w-2xl mx-auto mb-8">
          <h2 class="text-xl sm:text-2xl lg:text-[26px] font-extrabold text-brand-navy uppercase tracking-wide">
            Yêu Cầu Tư Vấn Báo Giá &amp; Kết Nối
          </h2>
          <div class="section-title-bar mx-auto"></div>
          <p class="mt-3 text-xs sm:text-sm text-slate-600">
            Để lại thông tin công trình của bạn, kỹ sư Dương Kiến Thành sẽ liên hệ tư vấn và gửi bảng báo giá chi tiết hoàn toàn miễn phí.
          </p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-start">

          <!-- Cột Trái: Form Yêu Cầu Tư Vấn & Báo Giá (Giống web mẫu Tín Trường Thịnh) -->
          <div class="lg:col-span-6 bg-white rounded-xl p-5 sm:p-7 border border-slate-200 shadow-sm">
            <h3 class="text-base sm:text-lg font-bold text-brand-navy mb-1">Gửi Yêu Cầu Tư Vấn &amp; Báo Giá</h3>
            <p class="text-xs text-slate-500 mb-5">Phản hồi nhanh chóng trong vòng 15 phút qua điện thoại hoặc Zalo.</p>

            <form id="quoteForm" onsubmit="handleQuoteSubmit(event)" class="space-y-3.5">
              <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                <div>
                  <label for="customerName" class="block text-xs font-semibold text-slate-700 mb-1">Họ và tên *</label>
                  <input id="customerName" type="text" required placeholder="Nhập họ tên của bạn" class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none" />
                </div>
                <div>
                  <label for="customerPhone" class="block text-xs font-semibold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                  <input id="customerPhone" type="tel" required placeholder="VD: 0905.198.539" class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none" />
                </div>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                <div>
                  <label for="projectType" class="block text-xs font-semibold text-slate-700 mb-1">Loại công trình</label>
                  <select id="projectType" class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none bg-white">
                    <option value="Nhà phố">Nhà phố</option>
                    <option value="Biệt thự">Biệt thự</option>
                    <option value="Khách sạn – Căn hộ – Phòng trọ">Khách sạn – Căn hộ – Phòng trọ</option>
                    <option value="Văn phòng">Văn phòng</option>
                    <option value="Thiết kế Kiến trúc">Thiết kế Kiến trúc</option>
                    <option value="Thi công phần thô">Thi công phần thô</option>
                    <option value="Thi công hoàn thiện">Thi công hoàn thiện</option>
                    <option value="Xây nhà trọn gói">Xây nhà trọn gói</option>
                    <option value="Cải tạo sửa chữa">Cải tạo sửa chữa</option>
                  </select>
                </div>
                <div>
                  <label for="investmentBudget" class="block text-xs font-semibold text-slate-700 mb-1">Mức đầu tư dự kiến</label>
                  <select id="investmentBudget" class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none bg-white">
                    <option value="Chưa xác định">Chưa xác định</option>
                    <option value="Dưới 500 triệu">Dưới 500 triệu</option>
                    <option value="500 triệu - 1 tỷ">500 triệu - 1 tỷ</option>
                    <option value="1 tỷ - 2 tỷ">1 tỷ - 2 tỷ</option>
                    <option value="2 tỷ - 3 tỷ">2 tỷ - 3 tỷ</option>
                    <option value="Trên 3 tỷ">Trên 3 tỷ</option>
                  </select>
                </div>
              </div>

              <div>
                <label for="customerEmail" class="block text-xs font-semibold text-slate-700 mb-1">Email (nếu có)</label>
                <input id="customerEmail" type="email" placeholder="example@gmail.com" class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none" />
              </div>

              <div>
                <label for="projectNote" class="block text-xs font-semibold text-slate-700 mb-1">Yêu cầu chi tiết (diện tích, số tầng, khu vực...)</label>
                <textarea id="projectNote" rows="3" placeholder="VD: Đất 5x20m tại Hòa Quý, dự kiến xây nhà phố 3 tầng trọn gói..." class="w-full px-3.5 py-2.5 text-sm rounded-lg border border-slate-300 focus:border-brand-navy focus:ring-1 focus:ring-brand-navy outline-none resize-y"></textarea>
              </div>

              <button type="submit" class="w-full py-3 px-5 rounded-lg bg-brand-navy hover:bg-brand-gold text-white font-bold text-sm transition-colors shadow-sm">
                Gửi Yêu Cầu Báo Giá Miễn Phí
              </button>

              <!-- Thông báo gửi form thành công (thay thế hoàn toàn alert) -->
              <div id="quoteSuccessBox" class="hidden rounded-lg bg-emerald-50 border border-emerald-200 p-3.5 text-xs sm:text-sm text-emerald-800">
                <strong>Gửi yêu cầu thành công!</strong> Cảm ơn quý khách đã liên hệ <strong>Dương Kiến Thành</strong>. Kỹ sư của chúng tôi sẽ gọi lại tư vấn qua số điện thoại bạn cung cấp trong thời gian sớm nhất.
              </div>
            </form>
          </div>

          <!-- Cột Phải: Bản Đồ Google Map & Facebook Fanpage Trực Tiếp Tại Trang Chủ -->
          <div class="lg:col-span-6 space-y-5">

            <!-- Bản đồ Google Maps tại Trang Chủ -->
            <div class="bg-white rounded-xl overflow-hidden border border-slate-200 shadow-sm">
              <div class="px-4 py-3 border-b border-slate-100 flex items-center justify-between gap-2">
                <div class="flex items-center gap-2 min-w-0">
                  <svg class="w-4 h-4 text-brand-gold shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                  <h3 class="text-sm font-bold text-brand-navy truncate">Bản Đồ Văn Phòng Công Ty</h3>
                </div>
                <a href="https://maps.google.com/?q=Khu+do+thi+Hoa+Quy+Ngu+Hanh+Son+Da+Nang" target="_blank" rel="noopener noreferrer" class="text-xs font-semibold text-brand-gold hover:underline whitespace-nowrap shrink-0">
                  Mở Google Maps
                </a>
              </div>
              <div class="w-full h-56 sm:h-64 bg-slate-100">
                <iframe
                  title="Bản đồ Công ty TNHH MTV Thiết Kế Và Xây Dựng Dương Kiến Thành"
                  src="https://maps.google.com/maps?q=Khu%20%C4%91%C3%B4%20th%E1%BB%8B%20H%C3%B2a%20Qu%C3%BD,%20Ng%C5%A9%20H%C3%A0nh%20S%C6%A1n,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=15&ie=UTF8&iwloc=&output=embed"
                  class="w-full h-full border-0"
                  loading="lazy"
                  referrerpolicy="no-referrer-when-downgrade">
                </iframe>
              </div>
              <div class="px-4 py-2.5 bg-slate-50 text-xs text-slate-600">
                <strong>Địa chỉ:</strong> Lô 41 B2.40 Khu đô thị Hòa Quý, Phường Ngũ Hành Sơn, Thành phố Đà Nẵng.
              </div>
            </div>

            <!-- Hộp Kết Nối Facebook Fanpage Trực Tiếp Tại Trang Chủ -->
            <div class="bg-white rounded-xl overflow-hidden border border-slate-200 shadow-sm">
              <div class="px-4 py-3 bg-[#1877F2] text-white flex items-center justify-between gap-2">
                <div class="flex items-center gap-2">
                  <svg class="w-4 h-4 fill-current shrink-0" viewBox="0 0 24 24"><path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/></svg>
                  <h3 class="text-sm font-bold">Fanpage Facebook Chính Thức</h3>
                </div>
                <span class="text-[11px] text-white/90">Cập nhật tiến độ hằng ngày</span>
              </div>

              <div class="p-4 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4">
                <div class="flex items-center gap-3">
                  <div class="w-12 h-12 rounded-lg bg-brand-navy flex items-center justify-center shrink-0 border border-brand-gold/40">
                    <svg class="w-8 h-8" viewBox="0 0 48 48" fill="none">
                      <path d="M6 36V19.5L24 8L42 19.5V36H35.5V22.8L24 15.6L12.5 22.8V36H6Z" fill="#D49E35"/>
                      <path d="M17 36V25.5L24 21L31 25.5V36H26.5V28.5H21.5V36H17Z" fill="#FFFFFF"/>
                      <rect x="6" y="38.5" width="36" height="2.5" rx="1.25" fill="#D49E35"/>
                    </svg>
                  </div>
                  <div>
                    <div class="text-sm font-bold text-brand-navy">Thiết Kế &amp; Xây Dựng Dương Kiến Thành</div>
                    <div class="text-xs text-slate-500 mt-0.5">facebook.com/duongkienthanh.xd • Đà Nẵng</div>
                    <div class="text-xs text-slate-600 mt-1">Theo dõi ảnh công trình thực tế &amp; nhận tư vấn trực tuyến qua Messenger.</div>
                  </div>
                </div>
                <div class="flex items-center gap-2 w-full sm:w-auto shrink-0">
                  <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" class="flex-1 sm:flex-none px-4 py-2 rounded-lg bg-[#1877F2] hover:bg-[#1465D1] text-white text-xs font-semibold text-center transition-colors whitespace-nowrap">
                    Theo Dõi Fanpage
                  </a>
                  <a href="https://m.me/" target="_blank" rel="noopener noreferrer" class="flex-1 sm:flex-none px-4 py-2 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-800 text-xs font-semibold text-center transition-colors whitespace-nowrap">
                    Nhắn Messenger
                  </a>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- ==================== FOOTER CHUYÊN NGHIỆP PHONG CÁCH FLATSOME ==================== -->
  <footer class="w-full bg-brand-navyDark text-slate-200 pt-10 pb-6 border-t-4 border-brand-gold">
    <div class="dkt-container">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-8 pb-8 border-b border-white/10">

        <!-- Cột 1: Thông tin công ty -->
        <div class="lg:col-span-5">
          <div class="flex items-center gap-2.5 mb-4">
            <div class="w-9 h-9 rounded-lg bg-brand-navy flex items-center justify-center border border-brand-gold/50 shrink-0">
              <svg class="w-6 h-6" viewBox="0 0 48 48" fill="none">
                <path d="M6 36V19.5L24 8L42 19.5V36H35.5V22.8L24 15.6L12.5 22.8V36H6Z" fill="#D49E35"/>
                <path d="M17 36V25.5L24 21L31 25.5V36H26.5V28.5H21.5V36H17Z" fill="#FFFFFF"/>
                <rect x="6" y="38.5" width="36" height="2.5" rx="1.25" fill="#D49E35"/>
              </svg>
            </div>
            <div>
              <div class="text-sm font-extrabold text-white tracking-tight">CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH</div>
              <div class="text-[11px] text-brand-goldLight font-medium">duongkienthanh.com</div>
            </div>
          </div>
          <ul class="space-y-2 text-xs sm:text-[13px] text-slate-300 leading-relaxed">
            <li><strong class="text-white">Trụ sở:</strong> Lô 41 B2.40 Khu đô thị Hòa Quý, Phường Ngũ Hành Sơn, Thành phố Đà Nẵng</li>
            <li><strong class="text-white">Hotline / Zalo:</strong> <a href="tel:0905198539" class="text-brand-goldLight hover:underline font-semibold">0905.198.539</a></li>
            <li><strong class="text-white">Website:</strong> <a href="https://duongkienthanh.com" class="hover:text-brand-goldLight">duongkienthanh.com</a></li>
            <li><strong class="text-white">Mã số thuế:</strong> 0402171855</li>
          </ul>
        </div>

        <!-- Cột 2: Lĩnh vực hoạt động -->
        <div class="lg:col-span-3">
          <h4 class="text-sm font-bold text-white uppercase tracking-wide mb-3.5">Lĩnh Vực Hoạt Động</h4>
          <ul class="space-y-2 text-xs sm:text-[13px] text-slate-300">
            <li><a href="#cong-trinh-thuc-te" onclick="filterProducts('thiet-ke-kien-truc')" class="hover:text-brand-goldLight transition-colors">Thiết kế Kiến trúc – Nội thất</a></li>
            <li><a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-phan-tho')" class="hover:text-brand-goldLight transition-colors">Thi công phần thô</a></li>
            <li><a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-hoan-thien')" class="hover:text-brand-goldLight transition-colors">Thi công hoàn thiện</a></li>
            <li><a href="#cong-trinh-thuc-te" onclick="filterProducts('thi-cong-noi-that')" class="hover:text-brand-goldLight transition-colors">Thi công nội thất</a></li>
            <li><a href="#du-an-da-nang" class="hover:text-brand-goldLight transition-colors">Dự án tại Đà Nẵng</a></li>
          </ul>
        </div>

        <!-- Cột 3: Danh mục báo giá -->
        <div class="lg:col-span-4">
          <h4 class="text-sm font-bold text-white uppercase tracking-wide mb-3.5">Báo Giá &amp; Hỗ Trợ Khách Hàng</h4>
          <ul class="space-y-2 text-xs sm:text-[13px] text-slate-300 mb-4">
            <li><a href="#bao-gia" class="hover:text-brand-goldLight transition-colors">Báo giá thiết kế kiến trúc</a></li>
            <li><a href="#bao-gia" class="hover:text-brand-goldLight transition-colors">Báo giá thi công phần thô</a></li>
            <li><a href="#bao-gia" class="hover:text-brand-goldLight transition-colors">Báo giá thi công hoàn thiện</a></li>
            <li><a href="#bao-gia" class="hover:text-brand-goldLight transition-colors">Báo giá xây nhà trọn gói Đà Nẵng</a></li>
          </ul>
          <p class="text-xs text-slate-400">Thời gian làm việc: Thứ 2 – Thứ 7 (07:30 – 17:30). Hỗ trợ tư vấn qua Hotline &amp; Zalo 24/7.</p>
        </div>

      </div>

      <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-xs text-slate-400">
        <p>Copyright © 2026 CÔNG TY TNHH MTV THIẾT KẾ VÀ XÂY DỰNG DƯƠNG KIẾN THÀNH.</p>
        <p>Thiết kế chuẩn giao diện Flatsome • duongkienthanh.com</p>
      </div>
    </div>
  </footer>

  <!-- ==================== CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI ==================== -->
  <div class="fixed right-3 sm:right-5 bottom-4 sm:bottom-6 z-50 flex flex-col items-end gap-2.5">
    <!-- Nút Zalo -->
    <a href="https://zalo.me/0905198539" target="_blank" rel="noopener noreferrer" aria-label="Chat Zalo 0905.198.539" class="group flex items-center gap-2 bg-[#0068FF] hover:bg-[#0056D6] text-white rounded-full shadow-lg pl-3 pr-3 sm:px-3.5 py-2.5 transition-all">
      <span class="w-6 h-6 rounded-full bg-white text-[#0068FF] font-extrabold text-[10px] flex items-center justify-center shrink-0">Zalo</span>
      <span class="hidden sm:inline text-xs font-bold whitespace-nowrap">Chat Zalo</span>
    </a>

    <!-- Nút Facebook -->
    <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" aria-label="Facebook Dương Kiến Thành" class="group flex items-center gap-2 bg-[#1877F2] hover:bg-[#1465D1] text-white rounded-full shadow-lg pl-3 pr-3 sm:px-3.5 py-2.5 transition-all">
      <svg class="w-6 h-6 fill-current shrink-0" viewBox="0 0 24 24"><path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/></svg>
      <span class="hidden sm:inline text-xs font-bold whitespace-nowrap">Facebook</span>
    </a>

    <!-- Nút Hotline -->
    <a href="tel:0905198539" aria-label="Gọi Hotline 0905.198.539" class="hotline-pulse flex items-center gap-2 bg-[#DC2626] hover:bg-[#B91C1C] text-white rounded-full shadow-lg px-3.5 py-2.5 transition-all">
      <svg class="w-5 h-5 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/></svg>
      <span class="text-xs font-bold whitespace-nowrap">0905.198.539</span>
    </a>
  </div>

  <!-- ==================== MODAL XEM CHI TIẾT CÔNG TRÌNH / BÀI VIẾT ==================== -->
  <div id="detailModal" class="fixed inset-0 z-50 hidden items-center justify-center bg-black/70 p-3 sm:p-5" onclick="closeModalOnBackdrop(event)">
    <div class="bg-white rounded-xl max-w-2xl w-full max-h-[90vh] overflow-y-auto shadow-2xl border border-slate-200">
      <div class="flex items-center justify-between px-4 sm:px-6 py-3.5 border-b border-slate-200 sticky top-0 bg-white z-10">
        <h3 id="modalTitle" class="text-sm sm:text-base font-bold text-brand-navy pr-4"></h3>
        <button type="button" onclick="closeDetailModal()" aria-label="Đóng" class="w-8 h-8 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-700 flex items-center justify-center shrink-0">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M6 18L18 6M6 6l12 12"/></svg>
        </button>
      </div>
      <div class="p-4 sm:p-6">
        <div id="modalImageWrap" class="w-full rounded-lg overflow-hidden bg-slate-100 mb-4 border border-slate-200">
          <img id="modalImage" src="" alt="" class="w-full max-h-[380px] object-cover" />
        </div>
        <div id="modalMeta" class="text-xs font-semibold text-brand-gold mb-2"></div>
        <p id="modalDesc" class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-5"></p>
        <div class="flex flex-wrap items-center gap-2.5 pt-3 border-t border-slate-100">
          <a href="#lien-he" onclick="closeDetailModal()" class="px-4 py-2.5 rounded-lg bg-brand-navy hover:bg-brand-gold text-white text-xs font-semibold transition-colors">
            Nhận Báo Giá Công Trình Tương Tự
          </a>
          <a href="tel:0905198539" class="px-4 py-2.5 rounded-lg bg-brand-goldSoft hover:bg-brand-gold hover:text-white text-brand-navy text-xs font-semibold transition-colors">
            Gọi Tư Vấn: 0905.198.539
          </a>
        </div>
      </div>
    </div>
  </div>

  <!-- ==================== JAVASCRIPT XỬ LÝ TƯƠNG TÁC ==================== -->
  <script>
    // Hàm tạo URL ảnh chất lượng cao từ Google Drive ID
    function getDriveThumb(fileId) {
      return `https://drive.google.com/thumbnail?id=${fileId}&sz=w1000`;
    }

    function getDriveFallback(fileId) {
      return `https://lh3.googleusercontent.com/d/${fileId}`;
    }

    // Xử lý tự động chuyển nguồn dự phòng nếu Google Drive bị giới hạn tải tạm thời
    function handleDriveImageError(imgEl, labelText) {
      try {
        const step = imgEl.getAttribute('data-err-step') || '0';
        const fallbackUrl = imgEl.getAttribute('data-fallback');
        if (step === '0' && fallbackUrl) {
          imgEl.setAttribute('data-err-step', '1');
          imgEl.src = fallbackUrl;
        } else {
          imgEl.onerror = null;
          const safeText = encodeURIComponent(labelText || 'Dương Kiến Thành');
          imgEl.src = `https://placehold.co/800x600/0F2A47/D49E35?text=${safeText}`;
        }
      } catch (e) {
        imgEl.onerror = null;
      }
    }

    // Dữ liệu 9 ảnh thực tế thi công xây dựng từ Google Drive của khách hàng
    const constructionProducts = [
      {
        id: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
        title: 'Thi Công Phần Thô Nhà Phố Hiện Đại',
        categoryLabel: 'Nhà phố • Thi công phần thô',
        categories: ['nha-pho', 'thi-cong-phan-tho'],
        desc: 'Hạng mục thi công phần thô nhà phố chuẩn kỹ thuật kết cấu móng, cột, dầm, sàn bê tông cốt thép do đội ngũ kỹ sư Dương Kiến Thành trực tiếp giám sát.'
      },
      {
        id: '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR',
        title: 'Thi Công Hoàn Thiện Biệt Thự Cao Cấp',
        categoryLabel: 'Biệt thự • Thi công hoàn thiện',
        categories: ['biet-thu', 'thi-cong-hoan-thien'],
        desc: 'Công trình biệt thự hoàn thiện mặt tiền sang trọng, hệ thống chống thấm, sơn nước ngoại thất và lắp đặt cửa nhôm kính sắc nét.'
      },
      {
        id: '1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv',
        title: 'Thiết Kế & Thi Công Nhà Phố 3 Tầng',
        categoryLabel: 'Nhà phố • Thiết kế kiến trúc',
        categories: ['nha-pho', 'thiet-ke-kien-truc', 'thi-cong-hoan-thien'],
        desc: 'Mẫu nhà phố 3 tầng hiện đại tối ưu ánh sáng tự nhiên và thông gió, bàn giao đúng tiến độ cam kết với chủ đầu tư.'
      },
      {
        id: '1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_',
        title: 'Thi Công Căn Hộ Cho Thuê – Khách Sạn',
        categoryLabel: 'Khách sạn – Căn hộ • Thi công trọn gói',
        categories: ['khach-san-can-ho', 'thi-cong-hoan-thien'],
        desc: 'Giải pháp thiết kế và thi công căn hộ dịch vụ, khách sạn tối ưu công năng khai thác cho thuê tại khu vực Đà Nẵng.'
      },
      {
        id: '1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO',
        title: 'Thi Công Nội Thất Trọn Gói Phòng Khách & Bếp',
        categoryLabel: 'Thi công nội thất • Nhà phố',
        categories: ['thi-cong-noi-that', 'nha-pho'],
        desc: 'Thi công hoàn thiện không gian nội thất tinh tế, vật liệu gỗ công nghiệp chống ẩm cao cấp kết hợp ánh sáng hài hòa.'
      },
      {
        id: '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t',
        title: 'Thi Công Kết Cấu Móng & Khung Bê Tông',
        categoryLabel: 'Thi công phần thô • Kết cấu',
        categories: ['thi-cong-phan-tho', 'nha-pho'],
        desc: 'Công tác gia công lắp dựng cốt thép, cốp pha và đổ bê tông đúng mác thiết kế, đảm bảo độ bền vững tuyệt đối cho công trình.'
      },
      {
        id: '1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_',
        title: 'Thiết Kế & Thi Công Văn Phòng Hiện Đại',
        categoryLabel: 'Văn phòng • Thi công nội thất',
        categories: ['van-phong', 'thi-cong-noi-that', 'thiet-ke-kien-truc'],
        desc: 'Không gian làm việc chuyên nghiệp, bố trí công năng khoa học, thi công nhanh gọn đáp ứng đúng tiến độ khai trương doanh nghiệp.'
      },
      {
        id: '1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT',
        title: 'Thi Công Biệt Thự 2 Mặt Tiền Sang Trọng',
        categoryLabel: 'Biệt thự • Thiết kế kiến trúc',
        categories: ['biet-thu', 'thiet-ke-kien-truc'],
        desc: 'Công trình biệt thự 2 mặt tiền bề thế với đường nét kiến trúc tinh xảo, sử dụng vật liệu hoàn thiện chất lượng cao.'
      },
      {
        id: '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn',
        title: 'Xây Nhà Trọn Gói Chìa Khóa Trao Tay',
        categoryLabel: 'Nhà phố • Thi công hoàn thiện',
        categories: ['nha-pho', 'thi-cong-hoan-thien'],
        desc: 'Dịch vụ xây dựng trọn gói từ khâu xin phép xây dựng, thiết kế, thi công phần thô đến hoàn thiện và bàn giao nhà ở.'
      }
    ];

    // Dữ liệu 10 ảnh dự án tại Đà Nẵng từ Google Drive của khách hàng
    const danangProjects = [
      {
        id: '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT',
        title: 'Nhà Phố Hiện Đại – KĐT Hòa Quý, Ngũ Hành Sơn',
        location: 'Phường Ngũ Hành Sơn, TP. Đà Nẵng',
        desc: 'Dự án thiết kế và xây dựng trọn gói nhà phố hiện đại tại Khu đô thị Hòa Quý với mặt tiền thoáng đẹp, đầy đủ công năng cho gia đình.'
      },
      {
        id: '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff',
        title: 'Biệt Thự Phố – KĐT Hòa Xuân, Cẩm Lệ',
        location: 'Quận Cẩm Lệ, TP. Đà Nẵng',
        desc: 'Công trình biệt thự phố thi công trọn gói tại Khu đô thị sinh thái Hòa Xuân, hoàn thiện sắc nét từng chi tiết.'
      },
      {
        id: '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz',
        title: 'Căn Hộ Dịch Vụ Cao Cấp – Quận Sơn Trà',
        location: 'Quận Sơn Trà, TP. Đà Nẵng',
        desc: 'Thi công căn hộ dịch vụ cho thuê gần biển Mỹ Khê, tối ưu diện tích phòng ốc và hệ thống điện nước vận hành ổn định.'
      },
      {
        id: '1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k',
        title: 'Nhà Phố 3 Tầng – Khu Nam Việt Á',
        location: 'Phường Ngũ Hành Sơn, TP. Đà Nẵng',
        desc: 'Nhà phố 3 tầng phong cách tối giản hiện đại, lấy sáng giếng trời thông thoáng tại khu dân cư Nam Việt Á.'
      },
      {
        id: '1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N',
        title: 'Khách Sạn Mini – Khu Vực Biển Mỹ Khê',
        location: 'TP. Đà Nẵng',
        desc: 'Dự án thi công phần thô và hoàn thiện khách sạn mini phục vụ du lịch, đảm bảo tiêu chuẩn phòng cháy và kết cấu bền vững.'
      },
      {
        id: '1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML',
        title: 'Nhà Phố 2 Mặt Tiền – Quận Hải Châu',
        location: 'Quận Hải Châu, TP. Đà Nẵng',
        desc: 'Nhà phố kết hợp kinh doanh tại trung tâm Hải Châu, thiết kế mặt tiền nổi bật, thi công an toàn trong khu dân cư đông đúc.'
      },
      {
        id: '1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF',
        title: 'Thi Công Văn Phòng – Quận Thanh Khê',
        location: 'Quận Thanh Khê, TP. Đà Nẵng',
        desc: 'Cải tạo và hoàn thiện trụ sở văn phòng làm việc hiện đại, tối ưu ánh sáng và âm thanh.'
      },
      {
        id: '1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A',
        title: 'Nhà Ở Gia Đình – Khu Đô Thị Phước Lý',
        location: 'Quận Liên Chiểu, TP. Đà Nẵng',
        desc: 'Xây nhà trọn gói cho gia đình trẻ tại Phước Lý, tối ưu ngân sách nhưng vẫn đảm bảo kiến trúc sang trọng.'
      },
      {
        id: '1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80',
        title: 'Biệt Thự Vườn – Khu Đô Thị FPT City',
        location: 'Phường Ngũ Hành Sơn, TP. Đà Nẵng',
        desc: 'Thiết kế và thi công biệt thự không gian xanh tại FPT City Đà Nẵng, hòa hợp giữa kiến trúc hiện đại và sân vườn.'
      },
      {
        id: '1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4',
        title: 'Nhà Phố Trọn Gói – Đường Lê Thiết Hùng',
        location: 'Hòa Xuân, TP. Đà Nẵng',
        desc: 'Công trình nhà phố hoàn thiện chìa khóa trao tay tại Hòa Xuân với vật tư hoàn thiện chính hãng và bảo hành chu đáo.'
      }
    ];

    // Dữ liệu các bài viết cẩm nang xây dựng trên trang chủ
    const blogArticles = [
      {
        title: 'Hướng dẫn bảo dưỡng bê tông móng và sàn đúng kỹ thuật',
        date: 'Cẩm nang kỹ thuật',
        imgId: '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t',
        excerpt: 'Bảo dưỡng bê tông đúng cách trong 7 ngày đầu quyết định trực tiếp đến cường độ chịu lực và hạn chế nứt bề mặt công trình.',
        content: 'Sau khi đổ bê tông móng, cột hoặc sàn, cần giữ ẩm liên tục trong ít nhất 7 ngày đầu bằng cách tưới nước phun sương nhẹ hoặc phủ bao bố ẩm. Tránh rung chấn mạnh khi bê tông chưa đạt cường độ tối thiểu. Tại Dương Kiến Thành, mọi công đoạn bảo dưỡng đều được kỹ sư kiểm tra ghi nhận mỗi ngày.'
      },
      {
        title: 'Kinh nghiệm xây nhà trọn gói tại Đà Nẵng không phát sinh chi phí',
        date: 'Kinh nghiệm xây nhà',
        imgId: '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn',
        excerpt: 'Chuẩn bị hồ sơ thiết kế chi tiết, bảng chủng loại vật tư rõ ràng và lựa chọn nhà thầu uy tín giúp chủ đầu tư chủ động hoàn toàn tài chính.',
        content: 'Để tránh phát sinh chi phí khi xây nhà, chủ đầu tư nên chốt kỹ mặt bằng công năng và phối cảnh 3D trước khi khởi công, thống nhất bảng vật liệu hoàn thiện theo từng thương hiệu cụ thể trong hợp đồng, đồng thời chọn đơn vị thi công có năng lực pháp lý và công trình thực tế rõ ràng tại Đà Nẵng.'
      },
      {
        title: 'Thiết kế nội thất nhà phố tối ưu ánh sáng và không gian sống',
        date: 'Xu hướng nội thất',
        imgId: '1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO',
        excerpt: 'Bố trí giếng trời, sử dụng gam màu sáng và nội thất thông minh giúp ngôi nhà ống tại đô thị luôn rộng rãi, thoáng đãng.',
        content: 'Đặc trưng của nhà phố tại các khu đô thị như Hòa Quý, Hòa Xuân là chiều ngang 5m và chiều sâu 18-20m. Việc kết hợp giếng trời giữa nhà, liên thông không gian phòng khách – bếp và dùng vật liệu gỗ tông ấm sẽ mang lại cảm giác thoáng đãng và sang trọng hơn hẳn.'
      },
      {
        title: '03 lưu ý quan trọng khi chuẩn bị thủ tục xin giấy phép xây dựng',
        date: 'Pháp lý xây dựng',
        imgId: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
        excerpt: 'Nắm rõ chỉ giới xây dựng, mật độ cho phép và chiều cao tầng theo quy hoạch giúp quá trình khởi công thuận lợi, đúng pháp luật.',
        content: 'Trước khi xây dựng, chủ nhà cần kiểm tra sổ đỏ, quy hoạch phân khu, mật độ xây dựng và khoảng lùi theo quy định địa phương. Khi ký hợp đồng thiết kế và thi công trọn gói tại Dương Kiến Thành, công ty hỗ trợ hoàn thiện hồ sơ xin phép xây dựng nhanh gọn cho khách hàng.'
      }
    ];

    // Render lưới sản phẩm / công trình thực tế (2 cột trên điện thoại, 3 cột trên máy tính, KHÔNG nhãn dán, tên hiển thị đầy đủ)
    function renderProducts(filterCat) {
      const container = document.getElementById('productGrid');
      if (!container) return;

      const list = filterCat === 'all'
        ? constructionProducts
        : constructionProducts.filter(item => item.categories.includes(filterCat));

      container.innerHTML = list.map((item, idx) => `
        <article
          onclick="openProductModal(${constructionProducts.indexOf(item)})"
          class="group bg-white rounded-xl overflow-hidden border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all cursor-pointer flex flex-col"
        >
          <div class="w-full aspect-[4/3] overflow-hidden bg-slate-100">
            <img
              src="${getDriveThumb(item.id)}"
              data-fallback="${getDriveFallback(item.id)}"
              alt="${item.title}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
              onerror="handleDriveImageError(this, '${item.title.replace(/'/g, '')}')"
            />
          </div>
          <div class="p-3 sm:p-4 flex-1 flex flex-col justify-between">
            <h3 class="text-[12.5px] sm:text-[14px] font-bold text-brand-navy group-hover:text-brand-gold transition-colors leading-snug break-words">
              ${item.title}
            </h3>
            <p class="mt-1.5 text-[11px] sm:text-xs text-slate-500 leading-snug break-words">
              ${item.categoryLabel}
            </p>
          </div>
        </article>
      `).join('');
    }

    // Chuyển tab danh mục
    function filterProducts(cat) {
      const buttons = document.querySelectorAll('.cat-tab');
      buttons.forEach(btn => {
        if (btn.getAttribute('data-cat') === cat) {
          btn.classList.remove('bg-white', 'text-slate-700', 'border-slate-200');
          btn.classList.add('bg-brand-navy', 'text-white', 'border-brand-navy');
        } else {
          btn.classList.remove('bg-brand-navy', 'text-white', 'border-brand-navy');
          btn.classList.add('bg-white', 'text-slate-700', 'border-slate-200');
        }
      });
      renderProducts(cat);
    }

    // Render 10 dự án tại Đà Nẵng
    function renderDanangProjects() {
      const container = document.getElementById('danangProjectGrid');
      if (!container) return;

      container.innerHTML = danangProjects.map((proj, idx) => `
        <article
          onclick="openDanangModal(${idx})"
          class="group bg-white rounded-xl overflow-hidden border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all cursor-pointer flex flex-col"
        >
          <div class="w-full aspect-[4/3] overflow-hidden bg-slate-100">
            <img
              src="${getDriveThumb(proj.id)}"
              data-fallback="${getDriveFallback(proj.id)}"
              alt="${proj.title}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
              onerror="handleDriveImageError(this, '${proj.title.replace(/'/g, '')}')"
            />
          </div>
          <div class="p-3 flex-1 flex flex-col justify-between">
            <h3 class="text-[12px] sm:text-[13px] font-bold text-brand-navy group-hover:text-brand-gold transition-colors leading-snug break-words">
              ${proj.title}
            </h3>
            <p class="mt-1.5 text-[11px] text-slate-500 leading-snug break-words">
              ${proj.location}
            </p>
          </div>
        </article>
      `).join('');
    }

    // Render danh mục các bài viết trang chủ
    function renderArticles() {
      const container = document.getElementById('articlesGrid');
      if (!container) return;

      container.innerHTML = blogArticles.map((art, idx) => `
        <article
          onclick="openArticleModal(${idx})"
          class="group bg-white rounded-xl overflow-hidden border border-slate-200 hover:border-brand-gold hover:shadow-md transition-all cursor-pointer flex flex-col"
        >
          <div class="w-full aspect-[16/10] overflow-hidden bg-slate-100">
            <img
              src="${getDriveThumb(art.imgId)}"
              data-fallback="${getDriveFallback(art.imgId)}"
              alt="${art.title}"
              loading="lazy"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
              onerror="handleDriveImageError(this, 'Tin Tức Xây Dựng')"
            />
          </div>
          <div class="p-3 sm:p-4 flex-1 flex flex-col">
            <span class="text-[11px] font-semibold text-brand-gold mb-1">${art.date}</span>
            <h3 class="text-[12.5px] sm:text-[14px] font-bold text-brand-navy group-hover:text-brand-gold transition-colors leading-snug break-words mb-1.5">
              ${art.title}
            </h3>
            <p class="text-[11.5px] sm:text-xs text-slate-600 leading-relaxed break-words">
              ${art.excerpt}
            </p>
          </div>
        </article>
      `).join('');
    }

    // Quản lý Modal xem chi tiết
    function openDetailModal(title, meta, desc, imgId) {
      const modal = document.getElementById('detailModal');
      const img = document.getElementById('modalImage');
      document.getElementById('modalTitle').textContent = title;
      document.getElementById('modalMeta').textContent = meta;
      document.getElementById('modalDesc').textContent = desc;
      img.removeAttribute('data-err-step');
      img.setAttribute('data-fallback', getDriveFallback(imgId));
      img.onerror = function () { handleDriveImageError(this, title); };
      img.src = getDriveThumb(imgId);
      modal.classList.remove('hidden');
      modal.classList.add('flex');
      document.body.style.overflow = 'hidden';
    }

    function openProductModal(index) {
      const item = constructionProducts[index];
      if (!item) return;
      openDetailModal(item.title, item.categoryLabel, item.desc, item.id);
    }

    function openDanangModal(index) {
      const proj = danangProjects[index];
      if (!proj) return;
      openDetailModal(proj.title, proj.location, proj.desc, proj.id);
    }

    function openArticleModal(index) {
      const art = blogArticles[index];
      if (!art) return;
      openDetailModal(art.title, art.date, art.content, art.imgId);
    }

    function closeDetailModal() {
      const modal = document.getElementById('detailModal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
      document.body.style.overflow = '';
    }

    function closeModalOnBackdrop(e) {
      if (e.target && e.target.id === 'detailModal') {
        closeDetailModal();
      }
    }

    // Xử lý 2 ảnh Banner tự trượt kích thước bằng nhau
    let currentSlide = 0;
    const totalSlides = 2;
    let slideTimer = null;

    function updateBannerSlides() {
      const slides = document.querySelectorAll('.banner-slide');
      slides.forEach((slide, idx) => {
        if (idx === currentSlide) {
          slide.classList.remove('is-inactive');
          slide.classList.add('is-active');
        } else {
          slide.classList.remove('is-active');
          slide.classList.add('is-inactive');
        }
      });

      for (let i = 0; i < totalSlides; i++) {
        const dot = document.getElementById(`dot-${i}`);
        if (!dot) continue;
        if (i === currentSlide) {
          dot.className = 'w-6 h-2 rounded-full bg-brand-gold transition-all';
        } else {
          dot.className = 'w-2.5 h-2 rounded-full bg-white/50 hover:bg-white transition-all';
        }
      }
    }

    function nextSlide() {
      currentSlide = (currentSlide + 1) % totalSlides;
      updateBannerSlides();
      resetSlideTimer();
    }

    function prevSlide() {
      currentSlide = (currentSlide - 1 + totalSlides) % totalSlides;
      updateBannerSlides();
      resetSlideTimer();
    }

    function goToSlide(idx) {
      currentSlide = idx;
      updateBannerSlides();
      resetSlideTimer();
    }

    function resetSlideTimer() {
      if (slideTimer) clearInterval(slideTimer);
      slideTimer = setInterval(() => {
        currentSlide = (currentSlide + 1) % totalSlides;
        updateBannerSlides();
      }, 5000);
    }

    // Menu điện thoại
    function toggleMobileMenu() {
      const menu = document.getElementById('mobileMenu');
      const openIcon = document.getElementById('menuIconOpen');
      const closeIcon = document.getElementById('menuIconClose');
      const isHidden = menu.classList.contains('hidden');
      if (isHidden) {
        menu.classList.remove('hidden');
        openIcon.classList.add('hidden');
        closeIcon.classList.remove('hidden');
      } else {
        menu.classList.add('hidden');
        openIcon.classList.remove('hidden');
        closeIcon.classList.add('hidden');
      }
    }

    function closeMobileMenu() {
      const menu = document.getElementById('mobileMenu');
      const openIcon = document.getElementById('menuIconOpen');
      const closeIcon = document.getElementById('menuIconClose');
      menu.classList.add('hidden');
      openIcon.classList.remove('hidden');
      closeIcon.classList.add('hidden');
    }

    // Tự chọn loại công trình khi bấm từ bảng báo giá
    function preselectQuote(typeName) {
      const select = document.getElementById('projectType');
      if (!select) return;
      for (let i = 0; i < select.options.length; i++) {
        if (select.options[i].value === typeName) {
          select.selectedIndex = i;
          break;
        }
      }
    }

    // Xử lý gửi form báo giá không dùng alert()
    function handleQuoteSubmit(event) {
      event.preventDefault();
      const successBox = document.getElementById('quoteSuccessBox');
      if (successBox) {
        successBox.classList.remove('hidden');
      }
      event.target.reset();
    }

    // Khởi tạo giao diện khi tải trang
    window.addEventListener('DOMContentLoaded', function () {
      renderProducts('all');
      renderDanangProjects();
      renderArticles();
      updateBannerSlides();
      resetSlideTimer();
    });
  </script>
</body>
</html>
