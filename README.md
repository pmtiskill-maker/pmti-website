<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title id="site-title">Premier Medical & Technical Institute (PMTI)</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Anek+Bangla:wght@400;500;600;700;800&family=Li+Ador+Noirrit&family=Poppins:wght@600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root { --primary-accent: #d97706; --primary-blue: #0284c7; --dark-navy: #0f172a; --text-dark: #1e293b; --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1); }
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { background: linear-gradient(rgba(248, 250, 252, 0.92), rgba(241, 245, 249, 0.95)), url('https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=1920&q=80') center/cover fixed no-repeat; color: var(--text-dark); font-family: 'Anek Bangla', sans-serif; overflow-x: hidden; min-height: 100vh; }
        h1, h2, h3 { font-family: 'Li Ador Noirrit', 'Anek Bangla', sans-serif; font-weight: 700; }
        .container { width: 100%; max-width: 1200px; margin: 0 auto; padding: 0 1rem; }
        .top-bar { background: #0f172a; color: #cbd5e1; padding: 0.5rem 0; font-size: 0.85rem; border-bottom: 1px solid rgba(255,255,255,0.1); }
        .top-bar .content { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 0.5rem; }
        .top-bar a { color: #fff; text-decoration: none; }
        header { background: #0f172a; position: sticky; top: 0; z-index: 1000; border-bottom: 3px solid var(--primary-accent); padding: 0.6rem 0; box-shadow: 0 4px 20px rgba(0,0,0,0.15); }
        .nav-wrapper { display: flex; flex-direction: column; align-items: center; gap: 0.8rem; }
        @media (min-width: 768px) { .nav-wrapper { flex-direction: row; justify-content: space-between; } }
        .logo-container { display: flex; flex-direction: column; align-items: center; text-decoration: none; gap: 0.5rem; text-align: center; }
        @media (min-width: 768px) { .logo-container { flex-direction: row; text-align: left; gap: 0.8rem; } }
        .official-logo-img { width: 65px; height: 65px; border-radius: 50%; object-fit: cover; border: 2px solid #d97706; }
        .logo-title-single { font-family: 'Poppins', sans-serif; font-size: 0.85rem; font-weight: 800; color: #fff; line-height: 1.2; }
        .logo-title-single span { color: #f59e0b; }
        .nav-menu { display: flex; list-style: none; gap: 0.8rem; align-items: center; flex-wrap: wrap; justify-content: center; }
        .nav-menu a { text-decoration: none; color: #f8fafc; font-weight: 600; font-size: 0.95rem; transition: var(--transition); cursor: pointer; }
        .nav-menu a:hover { color: #f59e0b; }
        .cart-btn-nav { background: rgba(255,255,255,0.1); color: #fff; border: 1px solid rgba(255,255,255,0.2); border-radius: 50px; padding: 0.5rem 1rem; cursor: pointer; display: flex; align-items: center; gap: 0.5rem; }
        .cart-count { background: #d97706; color: #fff; font-size: 0.75rem; font-weight: 800; border-radius: 50%; width: 20px; height: 20px; display: inline-flex; align-items: center; justify-content: center; }
        .btn { display: inline-flex; align-items: center; justify-content: center; gap: 0.5rem; padding: 0.65rem 1.2rem; border-radius: 50px; font-weight: 700; text-decoration: none; cursor: pointer; border: none; font-size: 0.9rem; transition: var(--transition); }
        .btn-primary { background: #d97706; color: #fff; }
        .btn-primary:hover { background: #b45309; }
        .btn-admin { background: #dc2626; color: #fff; }
        .btn-office { background: #0284c7; color: #fff; }
        .btn-outline { background: transparent; border: 2px solid #d97706; color: #d97706; }
        .btn-verify { background: #0284c7; color: #fff; }
        .btn-whatsapp { background: #16a34a; color: #fff; }
        .hidden-auth-box { display: none; background: #1e293b; padding: 0.8rem; text-align: center; border-bottom: 2px dashed #d97706; gap: 10px; justify-content: center; align-items: center; }
        .hidden-auth-box.show { display: flex; }
        .hero { padding: 3.5rem 0; }
        .hero-grid { display: grid; grid-template-columns: 1fr; gap: 2rem; align-items: center; }
        @media (min-width: 768px) { .hero-grid { grid-template-columns: 1.2fr 1fr; } }
        .hero-content h1 { font-size: 2.8rem; color: #0f172a; margin-bottom: 0.8rem; line-height: 1.3; }
        .hero-content h1 span { color: #d97706; }
        .hero-banner-card { background: #ffffff; border: 2px solid #cbd5e1; border-radius: 16px; padding: 1rem; box-shadow: 0 15px 30px rgba(0, 0, 0, 0.08); }
        .hero-banner-img { width: 100%; height: 230px; object-fit: cover; border-radius: 10px; display: block; }
        .section { padding: 3rem 0; }
        .section-title { text-align: center; margin-bottom: 2rem; }
        .section-title h2 { font-size: 2.2rem; color: #0f172a; position: relative; display: inline-block; }
        .section-title h2::after { content: ''; width: 50%; height: 4px; background: #d97706; position: absolute; bottom: -8px; left: 25%; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; }
        .card { background: rgba(255, 255, 255, 0.95); border-radius: 16px; overflow: hidden; display: flex; flex-direction: column; transition: var(--transition); box-shadow: 0 10px 25px rgba(0, 0, 0, 0.06); border: 1px solid #cbd5e1; }
        .card:hover { transform: translateY(-5px); border-color: #d97706; }
        .card img { width: 100%; height: 200px; object-fit: cover; cursor: pointer; }
        .card-body { padding: 1.4rem; flex-grow: 1; display: flex; flex-direction: column; }
        .badge { background: #fef3c7; color: #b45309; border: 1px solid #fde047; font-size: 0.8rem; font-weight: 700; padding: 0.3rem 0.7rem; border-radius: 50px; width: fit-content; margin-bottom: 0.6rem; }
        .card-title { font-size: 1.3rem; margin-bottom: 0.5rem; color: #0f172a; cursor: pointer; }
        .price-box { display: flex; align-items: center; gap: 10px; margin-bottom: 0.8rem; }
        .price { font-size: 1.3rem; font-weight: 800; color: #16a34a; }
        .old-price { font-size: 1rem; font-weight: 600; color: #94a3b8; text-decoration: line-through; }
        .view-page { display: none; }
        .view-page.active-page { display: block; }
        .admin-box { background: #fff; padding: 1.5rem; border-radius: 12px; border: 1px solid #cbd5e1; margin-bottom: 2rem; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .admin-table { width: 100%; border-collapse: collapse; margin-top: 1rem; }
        .admin-table th, .admin-table td { border: 1px solid #cbd5e1; padding: 0.6rem; text-align: left; font-size: 0.9rem; }
        .admin-table th { background: #f1f5f9; }
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(15, 23, 42, 0.75); backdrop-filter: blur(8px); z-index: 2000; justify-content: center; align-items: center; padding: 1rem; }
        .modal.active { display: flex; }
        .modal-content { background: #ffffff; border: 1px solid #cbd5e1; color: #0f172a; border-radius: 20px; max-width: 600px; width: 100%; padding: 1.8rem; position: relative; max-height: 90vh; overflow-y: auto; }
        .close-btn { position: absolute; top: 1rem; right: 1rem; font-size: 1.5rem; cursor: pointer; color: #64748b; width: 32px; height: 32px; background: #f1f5f9; border-radius: 50%; display: flex; align-items: center; justify-content: center; }
        .form-group { margin-bottom: 1rem; }
        .form-group label { display: block; font-size: 0.85rem; margin-bottom: 0.3rem; font-weight: 700; color: #0f172a; }
        .form-group input, .form-group select, .form-group textarea { width: 100%; padding: 0.75rem; background: #f8fafc; border: 1.5px solid #cbd5e1; border-radius: 8px; font-size: 0.95rem; font-family: inherit; }
        .detail-img { width: 100%; height: 220px; object-fit: cover; border-radius: 12px; margin-bottom: 1rem; }
        footer { background: #0f172a; color: #fff; padding: 3rem 0 1.5rem 0; margin-top: 3rem; text-align: center; }
    </style>
</head>
<body>
    <div class="top-bar">
        <div class="container content">
            <div><a href="tel:01306258338"><i class="fa-solid fa-phone"></i> 01306258338</a></div>
            <div><span><i class="fa-solid fa-certificate"></i> NSDA অনুমোদিত কারিগরি প্রতিষ্ঠান</span></div>
        </div>
    </div>
    <header>
        <div class="container nav-wrapper">
            <a href="#" class="logo-container" onclick="navigate('home')">
                <img id="header-logo" src="https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?auto=format&fit=crop&w=150&q=80" alt="Logo" class="official-logo-img">
                <div class="logo-title-single" id="header-title-text">
                    PREMIER MEDICAL &<br><span>TECHNICAL INSTITUTE</span>
                </div>
            </a>
            <ul class="nav-menu">
                <li><a onclick="navigate('home'); toggleSecretButtons();">হোম</a></li>
                <li><a onclick="navigate('courses')">কোর্সসমূহ</a></li>
                <li><a onclick="navigate('shop')">🛍️ শপ</a></li>
                <li>
                    <button class="cart-btn-nav" onclick="openCartModal()">
                        <i class="fa-solid fa-cart-shopping"></i>
                        <span class="cart-count" id="nav-cart-count">0</span>
                    </button>
                </li>
                <li><button class="btn btn-verify" onclick="openCertModal()"><i class="fa-solid fa-award"></i> সার্টিফিকেট</button></li>
            </ul>
        </div>
        <div id="secret-auth-box" class="hidden-auth-box">
            <button class="btn btn-admin" onclick="openLoginModal('admin')"><i class="fa-solid fa-lock"></i> এডমিন লগইন</button>
            <button class="btn btn-office" onclick="openLoginModal('office')"><i class="fa-solid fa-user-tie"></i> অফিস লগইন</button>
        </div>
    </header>
    <main>
        <div id="view-home" class="view-page active-page">
            <section class="hero">
                <div class="container hero-grid">
                    <div class="hero-content">
                        <h1>দক্ষতা অর্জন করুন,<br><span>আত্মনির্ভরশীল হয়ে উঠুন।</span></h1>
                        <p>Premier Medical & Technical Institute (PMTI)-এর মাধ্যমে বাস্তবমুখী কারিগরি শিক্ষা গ্রহণ করুন অথবা শিক্ষার্থীদের তৈরি হস্তশিল্প পণ্য সরাসরি অনলাইন শপ থেকে কেনাকাটা করুন।</p>
                        <div style="display: flex; gap: 0.8rem; flex-wrap: wrap;">
                            <button class="btn btn-primary" onclick="navigate('courses')">কোর্সসমূহ দেখুন</button>
                            <a href="https://wa.me/8801306258338" class="btn btn-whatsapp"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
                        </div>
                    </div>
                    <div class="hero-banner-card">
                        <img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=800&q=80" alt="Banner" class="hero-banner-img">
                    </div>
                </div>
            </section>
            <section class="section container">
                <div class="section-title"><h2>আমাদের মূল কোর্সসমূহ</h2></div>
                <div class="grid-3" id="courses-grid"></div>
            </section>
        </div>
        <div id="view-courses" class="view-page">
            <section class="section container">
                <div class="section-title"><h2>সবগুলো প্রফেশনাল কোর্স</h2></div>
                <div class="grid-3" id="all-courses-grid"></div>
            </section>
        </div>
        <div id="view-shop" class="view-page">
            <section class="section container">
                <div class="section-title"><h2>PMTI স্টুডেন্ট হস্তশিল্প শপ</h2></div>
                <div class="grid-3" id="shop-grid"></div>
            </section>
        </div>
        <div id="view-admin" class="view-page">
            <div class="container section">
                <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 1.5rem;">
                    <h2 id="dashboard-heading">⚙️ কন্ট্রোল প্যানেল</h2>
                    <button class="btn btn-outline" onclick="navigate('home')">হোমে ফিরে যান</button>
                </div>
                <div class="admin-box" id="admin-settings-section">
                    <h3>🌐 সাইটের লোগো, নাম ও ফুটার পরিবর্তন</h3>
                    <form onsubmit="updateGlobalSettings(event)" style="margin-top: 1rem;">
                        <div class="form-group"><label>প্রতিষ্ঠানের নাম</label><input type="text" id="setting-site-name" required></div>
                        <div class="form-group"><label>লোগো ছবির URL (Image Link)</label><input type="url" id="setting-logo-url" required></div>
                        <div class="form-group"><label>ফুটার কপিরাইট টেক্সট</label><input type="text" id="setting-footer-text" required></div>
                        <button type="submit" class="btn btn-primary">সেটিংস সেভ করুন</button>
                    </form>
                </div>
                <div class="admin-box">
                    <h3>🎓 স্টুডেন্ট তথ্য ও সার্টিফিকেট ম্যানেজমেন্ট</h3>
                    <form onsubmit="saveStudent(event)" style="margin-top: 1rem;">
                        <input type="hidden" id="edit-student-index" value="">
                        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem;">
                            <div class="form-group"><label>স্টুডেন্টের নাম</label><input type="text" id="stu-name" required></div>
                            <div class="form-group"><label>স্টুডেন্ট আইডি / রোল</label><input type="text" id="stu-id" required></div>
                            <div class="form-group"><label>সার্টিফিকেট নম্বর</label><input type="text" id="stu-cert" required></div>
                        </div>
                        <button type="submit" class="btn btn-primary" id="stu-save-btn">স্টুডেন্ট যোগ করুন</button>
                    </form>
                    <h4 style="margin-top: 1.5rem;">সংরক্ষিত স্টুডেন্ট তালিকা</h4>
                    <table class="admin-table">
                        <thead><tr><th>নাম</th><th>আইডি</th><th>সার্টিফিকেট নং</th><th>অ্যাকশন</th></tr></thead>
                        <tbody id="admin-student-list"></tbody>
                    </table>
                </div>
                <div class="admin-box" id="admin-courses-section">
                    <h3>➕ নতুন কোর্স যুক্ত করুন</h3>
                    <form onsubmit="addCourse(event)" style="margin-top: 1rem;">
                        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem;">
                            <div class="form-group"><label>কোর্সের নাম</label><input type="text" id="admin-c-title" required></div>
                            <div class="form-group"><label>ক্যাটাগরি</label><input type="text" id="admin-c-cat" required></div>
                            <div class="form-group"><label>বর্তমান ফি (টাকা)</label><input type="number" id="admin-c-price" required></div>
                            <div class="form-group"><label>পূর্বের ফি / ডিসকাউন্ট মূল্য (ঐচ্ছিক)</label><input type="number" id="admin-c-old-price"></div>
                            <div class="form-group"><label>মেয়াদ</label><input type="text" id="admin-c-dur" required value="আড়াই মাস"></div>
                            <div class="form-group"><label>ছবি URL</label><input type="url" id="admin-c-img" required></div>
                        </div>
                        <div class="form-group"><label>বিস্তারিত বিবরণ (কী কী শিখবেন ইত্যাদি)</label><textarea id="admin-c-desc" rows="3" required></textarea></div>
                        <button type="submit" class="btn btn-primary">কোর্স যোগ করুন</button>
                    </form>
                    <h4 style="margin-top: 1.5rem;">বর্তমান কোর্স তালিকা</h4>
                    <table class="admin-table">
                        <thead><tr><th>কোর্স</th><th>ফি</th><th>অ্যাকশন</th></tr></thead>
                        <tbody id="admin-course-list"></tbody>
                    </table>
                </div>
                <div class="admin-box" id="admin-products-section">
                    <h3>➕ নতুন শপ প্রোডাক্ট যুক্ত করুন</h3>
                    <form onsubmit="addProduct(event)" style="margin-top: 1rem;">
                        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem;">
                            <div class="form-group"><label>প্রোডাক্টের নাম</label><input type="text" id="admin-p-title" required></div>
                            <div class="form-group"><label>ক্যাটাগরি</label><input type="text" id="admin-p-cat" required></div>
                            <div class="form-group"><label>বর্তমান মূল্য (টাকা)</label><input type="number" id="admin-p-price" required></div>
                            <div class="form-group"><label>পূর্বের মূল্য / ডিসকাউন্ট (ঐচ্ছিক)</label><input type="number" id="admin-p-old-price"></div>
                            <div class="form-group"><label>ছবি URL</label><input type="url" id="admin-p-img" required></div>
                        </div>
                        <div class="form-group"><label>কালার (কমা দিয়ে লিখুন)</label><input type="text" id="admin-p-colors" placeholder="লাল, নীল"></div>
                        <div class="form-group"><label>সাইজ (কমা দিয়ে লিখুন)</label><input type="text" id="admin-p-sizes" placeholder="M, L, XL"></div>
                        <div class="form-group"><label>বিস্তারিত বিবরণ</label><textarea id="admin-p-desc" rows="3" required></textarea></div>
                        <button type="submit" class="btn btn-primary">প্রোডাক্ট যোগ করুন</button>
                    </form>
                    <h4 style="margin-top: 1.5rem;">বর্তমান প্রোডাক্ট তালিকা</h4>
                    <table class="admin-table">
                        <thead><tr><th>প্রোডাক্ট</th><th>মূল্য</th><th>অ্যাকশন</th></tr></thead>
                        <tbody id="admin-product-list"></tbody>
                    </table>
                </div>
            </div>
        </div>
    </main>
    <div class="modal" id="details-modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('details-modal')">&times;</span>
            <div id="details-modal-body"></div>
        </div>
    </div>
    <div class="modal" id="cart-modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('cart-modal')">&times;</span>
            <h3 style="margin-bottom: 1rem;"><i class="fa-solid fa-cart-shopping"></i> শপিং কার্ট ও পারচেজ</h3>
            <div id="cart-items-container"></div>
            <div style="margin-top: 1.5rem;" id="cart-footer">
                <h4>মোট মূল্য: <span id="cart-total-price" style="color: #16a34a;">৳0</span></h4>
                <div style="margin-top: 1rem; background:#f8fafc; padding:10px; border-radius:8px; border:1px solid #cbd5e1;">
                    <p style="font-size:0.9rem; font-weight:bold; margin-bottom:5px;">পেমেন্ট নির্দেশনা:</p>
                    <p style="font-size:0.85rem; color:#475569; margin-bottom:8px;">দয়া করে মোট টাকা নিচের নাম্বারে **সেন্ড মানি (Send Money)** করুন:<br><b style="color:#d97706; font-size:1.1rem;">📞 01306258338</b></p>
                    <div class="form-group" style="margin-bottom:0;">
                        <label>আপনার ট্রানজেকশন আইডি (TrxID) লিখুন</label>
                        <input type="text" id="trx-id-input" placeholder="যেমন: 9N7A6... ">
                    </div>
                </div>
                <button class="btn btn-primary" style="margin-top: 1rem; width:100%;" onclick="confirmOrder()">অর্ডার কনফার্ম করুন</button>
            </div>
        </div>
    </div>
    <div class="modal" id="cert-modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('cert-modal')">&times;</span>
            <h3>সার্টিফিকেট যাচাই</h3>
            <div class="form-group" style="margin-top: 1rem;">
                <label>স্টুডেন্ট আইডি বা সার্টিফিকেট নম্বর দিন</label>
                <input type="text" id="cert-search-input" placeholder="যেমন: 202601">
            </div>
            <button class="btn btn-primary" onclick="verifyCertificate()">যাচাই করুন</button>
            <div id="cert-result" style="margin-top: 1rem; font-weight: bold;"></div>
        </div>
    </div>
    <div class="modal" id="login-modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('login-modal')">&times;</span>
            <h3 id="login-modal-title">লগইন প্যানেল</h3>
            <form onsubmit="handleLoginSubmit(event)" style="margin-top: 1rem;">
                <div class="form-group"><label>পাসওয়ার্ড দিন</label><input type="password" id="login-pass-input" placeholder="পাসওয়ার্ড লিখুন" required></div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">লগইন</button>
            </form>
        </div>
    </div>
    <footer id="site-footer">
        <p>&copy; 2026 Premier Medical & Technical Institute (PMTI). All rights reserved.</p>
    </footer>
    <script>
        let siteSettings = JSON.parse(localStorage.getItem('pmti_settings')) || {
            name: "PREMIER MEDICAL & TECHNICAL INSTITUTE",
            logo: "https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?auto=format&fit=crop&w=150&q=80",
            footerText: "&copy; 2026 Premier Medical & Technical Institute (PMTI). All rights reserved."
        };
        let courses = JSON.parse(localStorage.getItem('pmti_courses')) || [
            { 
                id: 'c1', 
                title: 'ব্লক-বাটিক মাস্টারকোর্স', 
                category: 'ডিজাইন ও ফ্যাশন', 
                price: 4000, 
                oldPrice: 5500, 
                duration: 'আড়াই মাস', 
                image: 'https://images.unsplash.com/photo-1606041008023-472dfb5e530f?auto=format&fit=crop&w=600&q=80', 
                description: 'এই কোর্সে আপনি ঘরে বসে বা প্রফেশনাল পর্যায়ে আকর্ষণীয় বুটিক ব্যবসা শুরু করার পূর্ণাঙ্গ প্রশিক্ষণ পাবেন। আধুনিক ফ্যাশন ট্রেন্ড অনুযায়ী কাপড়ের ডিজাইন ও কালার কম্বিনেশন শিখিয়ে আত্মনির্ভরশীল করে তোলা হয়。<br><br><b>কী কী শিখবেন:</b><br>• প্রফেশনাল ব্লক প্রিন্টিং (কাঠ ও মেটাল ব্লক ব্যবহার)<br>• আকর্ষণীয় বাটিক ডিজাইন ও মোম বাটিকের কাজ<br>• টাই-ডাই ও স্ক্রিন প্রিন্টিংয়ের বেসিক কৌশল<br>• কাপড়ের মান নির্ণয় এবং কেমিক্যালের সঠিক মাত্রা<br>• নিজের বুটিক শপ পরিচালনা ও অনলাইন মার্কেটিং গাইডলাইন।' 
            },
            { 
                id: 'c2', 
                title: 'প্রফেশনাল টেইলরিং ও কাটিং', 
                category: 'গার্মেন্টস ও বুটিক', 
                price: 5000, 
                oldPrice: 6500, 
                duration: 'আড়াই মাস', 
                image: 'https://images.unsplash.com/photo-1558769132-cb1aea458c5e?auto=format&fit=crop&w=600&q=80', 
                description: 'সেলাইয়ের ভীতি দূর করে একদম জিরো থেকে নিখুঁত বডি মেজারমেন্ট, কাটিং এবং আকর্ষণীয় ফিটিংড পোশাক তৈরির আধুনিক প্র্যাকটিক্যাল কোর্স。<br><br><b>কী কী শিখবেন:</b><br>• সঠিক মাপে কাপড় কাটিং ও নিখুঁত সেলাই কৌশল<br>• থ্রি-পিস, কামিজ, ব্লাউজ ও পেটিকোট কাটিং<br>• বিভিন্ন স্টাইলের জেন্টস ও লেডিজ পোশাক তৈরি<br>• সেলাই মেশিনের সাধারণ ট্রাবলশুটিং ও মেইনটেন্যান্স<br>• কাস্টম অর্ডার নেওয়ার নিয়ম ও বুটিক ব্যবসার প্রারম্ভিক কৌশল।' 
            }
        ];
        let products = JSON.parse(localStorage.getItem('pmti_products')) || [
            { 
                id: 'p1', 
                title: 'হাতে তৈরি প্রিমিয়াম বাটিক থ্রি-পিস', 
                category: 'হস্তশিল্প ও বাটিক', 
                price: 1200, 
                oldPrice: 1600, 
                image: 'https://images.unsplash.com/photo-1610030469983-98e550d6193c?auto=format&fit=crop&w=600&q=80', 
                colors: ['লাল-কালো', 'নীল-সাদা', 'মেরুন-গোল্ডেন'], 
                sizes: ['Medium', 'Large', 'Semi-Long'], 
                description: 'আমাদের প্রতিষ্ঠানের দক্ষ শিক্ষার্থীদের নিখুঁত হাতের কাজ ও প্রিমিয়াম কোয়ালিটির সুতি কাপড়ের তৈরি আকর্ষণীয় বাটিক থ্রি-পিস। গরমে আরামদায়ক এবং সব বয়সিদের ব্যবহারের উপযোগী।' 
            }
        ];
        let students = JSON.parse(localStorage.getItem('pmti_students')) || [
            { name: 'রহিম উদ্দিন', id: '202601', cert: 'REG-101' }
        ];
        let cart = [];
        let currentRole = '';
        function saveAll() {
            localStorage.setItem('pmti_settings', JSON.stringify(siteSettings));
            localStorage.setItem('pmti_courses', JSON.stringify(courses));
            localStorage.setItem('pmti_products', JSON.stringify(products));
            localStorage.setItem('pmti_students', JSON.stringify(students));
            renderAll();
        }
        function renderAll() {
            document.getElementById('header-logo').src = siteSettings.logo;
            document.getElementById('header-title-text').innerHTML = siteSettings.name.replace('&', '<br><span>') + '</span>';
            document.getElementById('site-title').innerText = siteSettings.name;
            document.getElementById('site-footer').innerHTML = `<p>${siteSettings.footerText}</p>`;
            const cHtml = courses.map(c => `
                <div class="card">
                    <img src="${c.image}" alt="${c.title}" onclick="showCourseModal('${c.id}')">
                    <div class="card-body">
                        <span class="badge">${c.category}</span>
                        <h3 class="card-title" onclick="showCourseModal('${c.id}')">${c.title}</h3>
                        <p style="color:#64748b; font-size:0.9rem; margin-bottom:0.5rem;">মেয়াদ: ${c.duration}</p>
                        <div class="price-box">
                            <span class="price">৳${c.price}</span>
                            ${c.oldPrice ? `<span class="old-price">৳${c.oldPrice}</span>` : ''}
                        </div>
                        <button class="btn btn-primary" style="width:100%;" onclick="showCourseModal('${c.id}')"><i class="fa-solid fa-graduation-cap"></i> এনরোল করুন (Enroll Now)</button>
                    </div>
                </div>
            `).join('');
            document.getElementById('courses-grid').innerHTML = cHtml;
            document.getElementById('all-courses-grid').innerHTML = cHtml;
            const pHtml = products.map(p => `
                <div class="card">
                    <img src="${p.image}" alt="${p.title}" onclick="showProductModal('${p.id}')">
                    <div class="card-body">
                        <span class="badge">${p.category}</span>
                        <h3 class="card-title" onclick="showProductModal('${p.id}')">${p.title}</h3>
                        <div class="price-box">
                            <span class="price">৳${p.price}</span>
                            ${p.oldPrice ? `<span class="old-price">৳${p.oldPrice}</span>` : ''}
                        </div>
                        <button class="btn btn-primary" style="width:100%;" onclick="showProductModal('${p.id}')"><i class="fa-solid fa-circle-info"></i> বিস্তারিত ও কিনুন</button>
                    </div>
                </div>
            `).join('');
            document.getElementById('shop-grid').innerHTML = pHtml;
            document.getElementById('admin-course-list').innerHTML = courses.map((c, i) => `
                <tr><td>${c.title}</td><td>৳${c.price}</td><td><button style="color:red; cursor:pointer; border:none; background:none; font-weight:bold;" onclick="deleteCourse(${i})">ডিলিট</button></td></tr>
            `).join('');
            document.getElementById('admin-product-list').innerHTML = products.map((p, i) => `
                <tr><td>${p.title}</td><td>৳${p.price}</td><td><button style="color:red; cursor:pointer; border:none; background:none; font-weight:bold;" onclick="deleteProduct(${i})">ডিলিট</button></td></tr>
            `).join('');
            renderStudentTable();
        }
        function renderStudentTable() {
            document.getElementById('admin-student-list').innerHTML = students.map((s, i) => `
                <tr>
                    <td>${s.name}</td><td>${s.id}</td><td>${s.cert}</td>
                    <td>
                        <button class="btn" style="padding:4px 8px; font-size:0.8rem; background:#0284c7;" onclick="editStudent(${i})">এডিট</button>
                        <button class="btn" style="padding:4px 8px; font-size:0.8rem; background:#dc2626;" onclick="deleteStudent(${i})">ডিলিট</button>
                    </td>
                </tr>
            `).join('');
        }
        function toggleSecretButtons() {
            document.getElementById('secret-auth-box').classList.toggle('show');
        }
        function openLoginModal(role) {
            currentRole = role;
            document.getElementById('login-modal-title').innerText = role === 'admin' ? 'এডমিন প্যানেল লগইন' : 'অফিস প্যানেল লগইন';
            document.getElementById('login-pass-input').value = '';
            document.getElementById('login-modal').classList.add('active');
            document.getElementById('secret-auth-box').classList.remove('show');
        }
        function handleLoginSubmit(e) {
            e.preventDefault();
            const pass = document.getElementById('login-pass-input').value;
            if (currentRole === 'admin' && pass === 'abrar321') {
                closeModal('login-modal');
                setupAdminDashboard(true);
                navigate('admin');
            } else if (currentRole === 'office' && pass === 'abrar123') {
                closeModal('login-modal');
                setupAdminDashboard(false);
                navigate('admin');
            } else {
                alert('ভুল পাসওয়ার্ড!');
            }
        }
        function setupAdminDashboard(isAdmin) {
            if (isAdmin) {
                document.getElementById('dashboard-heading').innerText = '⚙️ এডমিন কন্ট্রোল প্যানেল';
                document.getElementById('admin-settings-section').style.display = 'block';
                document.getElementById('admin-courses-section').style.display = 'block';
                document.getElementById('admin-products-section').style.display = 'block';
                document.getElementById('setting-site-name').value = siteSettings.name;
                document.getElementById('setting-logo-url').value = siteSettings.logo;
                document.getElementById('setting-footer-text').value = siteSettings.footerText;
            } else {
                document.getElementById('dashboard-heading').innerText = '🏢 অফিস কন্ট্রোল প্যানেল (স্টুডেন্ট ডাটা ম্যানেজমেন্ট)';
                document.getElementById('admin-settings-section').style.display = 'none';
                document.getElementById('admin-courses-section').style.display = 'none';
                document.getElementById('admin-products-section').style.display = 'none';
            }
        }
        function updateGlobalSettings(e) {
            e.preventDefault();
            siteSettings.name = document.getElementById('setting-site-name').value;
            siteSettings.logo = document.getElementById('setting-logo-url').value;
            siteSettings.footerText = document.getElementById('setting-footer-text').value;
            saveAll();
            alert('সেটিংস সফলভাবে আপডেট হয়েছে!');
        }
        function saveStudent(e) {
            e.preventDefault();
            const name = document.getElementById('stu-name').value;
            const id = document.getElementById('stu-id').value;
            const cert = document.getElementById('stu-cert').value;
            const editIndex = document.getElementById('edit-student-index').value;
            if (editIndex === "") students.push({ name, id, cert });
            else {
                students[editIndex] = { name, id, cert };
                document.getElementById('edit-student-index').value = "";
                document.getElementById('stu-save-btn').innerText = 'স্টুডেন্ট যোগ করুন';
            }
            saveAll();
            e.target.reset();
            alert('সফলভাবে সংরক্ষিত হয়েছে!');
        }
        function editStudent(i) {
            document.getElementById('stu-name').value = students[i].name;
            document.getElementById('stu-id').value = students[i].id;
            document.getElementById('stu-cert').value = students[i].cert;
            document.getElementById('edit-student-index').value = i;
            document.getElementById('stu-save-btn').innerText = 'তথ্য আপডেট করুন';
        }
        function deleteStudent(i) {
            if(confirm('ডিলেট করতে চান?')) { students.splice(i, 1); saveAll(); }
        }
        function addCourse(e) {
            e.preventDefault();
            courses.push({
                id: 'c' + Date.now(),
                title: document.getElementById('admin-c-title').value,
                category: document.getElementById('admin-c-cat').value,
                price: Number(document.getElementById('admin-c-price').value),
                oldPrice: document.getElementById('admin-c-old-price').value ? Number(document.getElementById('admin-c-old-price').value) : null,
                duration: document.getElementById('admin-c-dur').value,
                image: document.getElementById('admin-c-img').value,
                description: document.getElementById('admin-c-desc').value
            });
            saveAll(); e.target.reset(); alert('কোর্স যোগ করা হয়েছে!');
        }
        function addProduct(e) {
            e.preventDefault();
            products.push({
                id: 'p' + Date.now(),
                title: document.getElementById('admin-p-title').value,
                category: document.getElementById('admin-p-cat').value,
                price: Number(document.getElementById('admin-p-price').value),
                oldPrice: document.getElementById('admin-p-old-price').value ? Number(document.getElementById('admin-p-old-price').value) : null,
                image: document.getElementById('admin-p-img').value,
                colors: document.getElementById('admin-p-colors').value.split(',').map(s=>s.trim()),
                sizes: document.getElementById('admin-p-sizes').value.split(',').map(s=>s.trim()),
                description: document.getElementById('admin-p-desc').value
            });
            saveAll(); e.target.reset(); alert('প্রোডাক্ট যোগ করা হয়েছে!');
        }
        function deleteCourse(i) { courses.splice(i, 1); saveAll(); }
        function deleteProduct(i) { products.splice(i, 1); saveAll(); }
        function showCourseModal(id) {
            const c = courses.find(item => item.id === id);
            document.getElementById('details-modal-body').innerHTML = `
                <img src="${c.image}" class="detail-img">
                <h2>${c.title}</h2>
                <p style="margin: 0.5rem 0; font-size:0.9rem; color:#64748b;">ক্যাটাগরি: ${c.category} | মেয়াদ: ${c.duration}</p>
                <div class="price-box">
                    <span class="price">৳${c.price}</span>
                    ${c.oldPrice ? `<span class="old-price">৳${c.oldPrice}</span>` : ''}
                </div>
                <div style="background:#f8fafc; padding:12px; border-radius:8px; margin-bottom:1rem; border:1px solid #e2e8f0;">
                    <h4 style="margin-bottom:5px; font-size:1rem;">কোর্সের বিস্তারিত বিবরণ ও শিখনফল:</h4>
                    <p style="color:#334155; font-size:0.95rem; line-height:1.6;">${c.description}</p>
                </div>
                <button class="btn btn-primary" style="width:100%;" onclick="addToCart('${c.id}', 'course'); closeModal('details-modal');"><i class="fa-solid fa-graduation-cap"></i> এনরোল করুন (Enroll Now)</button>
            `;
            document.getElementById('details-modal').classList.add('active');
        }
        function showProductModal(id) {
            const p = products.find(item => item.id === id);
            document.getElementById('details-modal-body').innerHTML = `
                <img src="${p.image}" class="detail-img">
                <h2>${p.title}</h2>
                <div class="price-box" style="margin-top:5px;">
                    <span class="price">৳${p.price}</span>
                    ${p.oldPrice ? `<span class="old-price">৳${p.oldPrice}</span>` : ''}
                </div>
                <p style="color:#475569; font-size:0.95rem; margin-bottom:1rem; line-height:1.5;">${p.description}</p>
                <div style="display:grid; grid-template-columns: 1fr 1fr; gap:10px;">
                    <div class="form-group"><label>কালার সিলেক্ট করুন:</label><select id="modal-p-col">${(p.colors||[]).map(col=>`<option>${col}</option>`)}</select></div>
                    <div class="form-group"><label>সাইজ সিলেক্ট করুন:</label><select id="modal-p-size">${(p.sizes||[]).map(sz=>`<option>${sz}</option>`)}</select></div>
                </div>
                <div class="form-group"><label>পরিমাণ (Quantity):</label><input type="number" id="modal-p-qty" value="1" min="1" max="10"></div>
                <button class="btn btn-primary" style="width:100%;" onclick="addProductToCart('${p.id}'); closeModal('details-modal');">কার্টে রাখুন</button>
            `;
            document.getElementById('details-modal').classList.add('active');
        }
        function addToCart(id, type) {
            let item = courses.find(c => c.id === id);
            cart.push({ ...item, qty: 1, type: 'course' });
            document.getElementById('nav-cart-count').innerText = cart.length;
            alert('কোর্সটি সফলভাবে এনরোলমেন্টের জন্য কার্টে যুক্ত করা হয়েছে!');
        }
        function addProductToCart(id) {
            let p = products.find(item => item.id === id);
            let col = document.getElementById('modal-p-col').value;
            let sz = document.getElementById('modal-p-size').value;
            let qty = Number(document.getElementById('modal-p-qty').value);
            cart.push({ ...p, selectedColor: col, selectedSize: sz, qty: qty, type: 'product' });
            document.getElementById('nav-cart-count').innerText = cart.length;
            alert('প্রোডাক্টটি কার্টে যুক্ত করা হয়েছে!');
        }
        function openCartModal() {
            const container = document.getElementById('cart-items-container');
            container.innerHTML = cart.length === 0 ? '<p>আপনার কার্ট খালি!</p>' : cart.map((i, index) => `
                <div style="display:flex; justify-content:space-between; align-items:center; padding:8px 0; border-bottom:1px solid #e2e8f0;">
                    <div>
                        <b>${i.title}</b><br>
                        <small style="color:#64748b;">${i.selectedColor ? `কালার: ${i.selectedColor}, ` : ''} ${i.selectedSize ? `সাইজ: ${i.selectedSize}, ` : ''} পরিমাণ: ${i.qty}</small>
                    </div>
                    <div style="text-align:right;">
                        <b>৳${i.price * i.qty}</b><br>
                        <button style="color:red; background:none; border:none; cursor:pointer; font-size:0.8rem;" onclick="removeFromCart(${index})">রিমুভ</button>
                    </div>
                </div>
            `).join('');
            let total = cart.reduce((sum, i) => sum + (i.price * i.qty), 0);
            document.getElementById('cart-total-price').innerText = '৳' + total;
            document.getElementById('cart-modal').classList.add('active');
        }
        function removeFromCart(index) {
            cart.splice(index, 1);
            document.getElementById('nav-cart-count').innerText = cart.length;
            openCartModal();
        }
        function confirmOrder() {
            let trx = document.getElementById('trx-id-input').value.trim();
            if(cart.length === 0) { alert('কার্ট খালি!'); return; }
            if(!trx) { alert('দয়া করে আপনার ট্রানজেকশন আইডি (TrxID) লিখুন।'); return; }
            alert('ধন্যবাদ! আপনার অর্ডারটি সফলভাবে সাবমিট হয়েছে। TrxID যাচাই করে দ্রুত কনফার্ম করা হবে।');
            cart = [];
            document.getElementById('nav-cart-count').innerText = '0';
            document.getElementById('trx-id-input').value = '';
            closeModal('cart-modal');
        }
        function verifyCertificate() {
            const val = document.getElementById('cert-search-input').value.trim();
            const resBox = document.getElementById('cert-result');
            if(!val) { resBox.innerHTML = "<span style='color:red;'>আইডি বা সার্টিফিকেট নাম্বার দিন।</span>"; return; }
            const found = students.find(s => s.id === val || s.cert === val);
            if(found) {
                resBox.innerHTML = `<div style="background:#f0fdf4; border:1px solid #bbf7d0; padding:10px; border-radius:6px; color:#16a34a;">
                    ✅ সার্টিফিকেট বৈধ!<br>নাম: ${found.name}<br>আইডি: ${found.id}<br>সার্টিফিকেট নং: ${found.cert}
                </div>`;
            } else {
                resBox.innerHTML = `<span style='color:red;'>❌ কোনো তথ্য পাওয়া যায়নি!</span>`;
            }
        }
        function navigate(pageId) {
            document.querySelectorAll('.view-page').forEach(el => el.classList.remove('active-page'));
            document.getElementById('view-' + pageId).classList.add('active-page');
            window.scrollTo(0, 0);
        }
        function closeModal(id) { document.getElementById(id).classList.remove('active'); }
        function openCertModal() { document.getElementById('cert-modal').classList.add('active'); }
        renderAll();
    </script>
</body>
</html>
