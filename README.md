Huyền_Speaking_1-100
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Luyện 100 Từ Vựng IELTS - Red Edition Pro</title>
    <style>
        :root {
            --primary-color: #d32f2f;
            --secondary-color: #b71c1c;
            --accent-light: #ffebee;
            --bg-color: #fdf2f2;
            --card-bg: #ffffff;
            --text-color: #333333;
            --success-color: #2e7d32;
            --warning-color: #f57f17;
            --gray-color: #757575;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            color: var(--text-color);
            padding: 10px;
            box-sizing: border-box;
        }

        .container {
            background-color: var(--card-bg);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(211, 47, 47, 0.15);
            width: 100%;
            max-width: 500px;
            text-align: center;
            border-top: 5px solid var(--primary-color);
            position: relative;
            box-sizing: border-box;
        }

        /* Header & Progress */
        .header-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .header-controls {
            display: flex;
            gap: 10px;
        }

        .btn-icon {
            background: none;
            border: none;
            font-size: 22px; 
            cursor: pointer;
            color: var(--primary-color);
            padding: 5px;
            transition: transform 0.2s;
        }
        .btn-icon:hover { transform: scale(1.1); }

        .progress-bar {
            color: #ef5350;
            font-weight: 600;
            font-size: 14px;
            letter-spacing: 1px;
        }

        /* Card Area */
        .card {
            min-height: 280px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
        }

        .vietnamese-text {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
            color: #2c3e50;
            line-height: 1.4;
            word-wrap: break-word; 
        }

        .hidden-content {
            display: none;
            animation: fadeIn 0.5s ease-out;
            width: 100%;
        }

        /* Layout cho hàng chứa từ tiếng Anh và nút loa */
        .english-row {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin: 5px 0; 
            flex-wrap: wrap;
        }

        .english-word {
            font-size: 32px;
            color: var(--primary-color);
            font-weight: 800;
            text-shadow: 1px 1px 0px rgba(0,0,0,0.05);
            margin: 0;
            word-break: break-word; 
        }

        /* Style cho phiên âm IPA */
        .ipa-text {
            font-family: 'Lucida Sans Unicode', 'Arial Unicode MS', sans-serif;
            font-size: 18px;
            color: #757575;
            margin-bottom: 10px;
            font-weight: 400;
        }

        /* Nút nghe lại âm thanh */
        .btn-audio-replay {
            background: white;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
            width: 40px; 
            height: 40px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.2s;
            flex-shrink: 0;
            -webkit-tap-highlight-color: transparent; 
        }
        .btn-audio-replay:hover {
            background: var(--primary-color);
            color: white;
            transform: scale(1.1);
        }

        .part-of-speech {
            font-style: italic;
            color: #c62828;
            margin-bottom: 5px;
            font-size: 14px;
            background: var(--accent-light);
            padding: 5px 12px;
            border-radius: 15px;
            display: inline-block;
            border: 1px solid #ffcdd2;
        }

        /* FIX: Ensure example box style is present */
        .example-box {
            font-size: 16px;
            color: #4b5563;
            margin-top: 15px;
            padding: 15px;
            background-color: #fff5f5;
            border-left: 4px solid var(--primary-color);
            border-radius: 0 8px 8px 0;
            text-align: left;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            line-height: 1.5;
            display: none; /* Hidden by default */
        }

        /* Buttons */
        .btn {
            border: none;
            padding: 14px 20px; 
            font-size: 16px;
            font-weight: 600;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            color: white;
            -webkit-tap-highlight-color: transparent;
        }
        
        .btn:hover { transform: translateY(-2px); box-shadow: 0 6px 12px rgba(0,0,0,0.15); }
        .btn:active { transform: translateY(1px); }
        .btn:disabled { background: #bdbdbd !important; cursor: not-allowed; transform: none; box-shadow: none; color: #fff;}

        .btn-reveal {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            width: 100%;
            margin-top: 20px;
            font-size: 18px;
        }

        /* Navigation Row */
        .nav-row {
            display: flex;
            justify-content: space-between;
            margin-top: 25px;
            gap: 15px;
        }

        .btn-nav {
            background-color: white;
            color: var(--primary-color);
            border: 2px solid var(--primary-color);
            width: 55px; 
            height: 55px;
            border-radius: 50%;
            font-size: 22px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0;
        }

        /* Review Status Buttons */
        .review-actions {
            display: flex;
            gap: 10px;
            margin-top: 20px;
            justify-content: center;
        }

        .btn-learn { background-color: var(--warning-color); flex: 1; }
        .btn-success { background-color: var(--success-color); flex: 1; }

        .status-badge {
            font-size: 12px;
            padding: 4px 8px;
            border-radius: 4px;
            margin-bottom: 10px;
            display: inline-block;
            font-weight: bold;
        }
        .status-new { color: var(--gray-color); background: #eee; }
        .status-learned { color: var(--success-color); background: #e8f5e9; border: 1px solid #c8e6c9; }
        .status-learning { color: var(--warning-color); background: #fff3e0; border: 1px solid #ffe0b2; }

        .status-msg {
            font-size: 13px;
            margin-top: 10px;
            color: #e53935;
            font-style: italic;
            height: 20px;
        }

        /* Modal Global */
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.6);
            z-index: 100;
            justify-content: center;
            align-items: center;
            backdrop-filter: blur(2px);
        }

        .modal-content {
            background: white;
            width: 90%;
            max-width: 400px;
            max-height: 85vh; 
            border-radius: 15px;
            padding: 20px;
            display: flex;
            flex-direction: column;
            box-shadow: 0 20px 50px rgba(0,0,0,0.3);
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }

        /* List Modal Styles */
        .list-container {
            overflow-y: auto;
            flex: 1;
            -webkit-overflow-scrolling: touch; 
        }

        .list-item {
            display: flex;
            justify-content: space-between;
            padding: 12px 10px; 
            border-bottom: 1px solid #f5f5f5;
            cursor: pointer;
            text-align: left;
            align-items: center;
        }
        .list-item:hover { background-color: #fce4ec; }
        .list-item.active { background-color: #ffcdd2; font-weight: bold; }

        /* Stats Modal Styles */
        .stats-summary {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            text-align: center;
        }
        .stat-box {
            padding: 10px;
            border-radius: 10px;
            width: 30%;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }
        .stat-val { font-size: 20px; font-weight: bold; display: block; }
        .stat-label { font-size: 12px; }
        
        .bg-learned { background: #e8f5e9; color: var(--success-color); }
        .bg-learning { background: #fff3e0; color: var(--warning-color); }
        .bg-new { background: #f5f5f5; color: var(--gray-color); }

        .recommend-section {
            text-align: left;
            margin-top: 10px;
            flex: 1;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
        }
        .recommend-item {
            padding: 12px 8px;
            border-bottom: 1px solid #eee;
            cursor: pointer;
            color: var(--warning-color);
            font-weight: 500;
        }
        .recommend-item:hover { background: #fff3e0; }
        
        /* Settings Modal Custom */
        .settings-row {
            margin-bottom: 15px;
            text-align: left;
        }
        .settings-label {
            font-weight: 600;
            margin-bottom: 5px;
            display: block;
            color: #555;
        }
        select.settings-input {
            width: 100%;
            padding: 10px;
            border-radius: 8px;
            border: 1px solid #ccc;
            font-size: 14px;
            background: #fff;
        }
        input[type=range] {
            width: 100%;
            margin-top: 5px;
        }

        /* --- RESPONSIVE MOBILE CONFIGURATION --- */
        @media (max-width: 480px) {
            .container {
                padding: 20px;
            }
            .vietnamese-text { font-size: 20px; }
            .english-word { font-size: 26px; }
            .card { min-height: 240px; }
            .btn { font-size: 15px; padding: 12px; }
            .btn-nav { width: 45px; height: 45px; font-size: 18px; }
            .header-controls { gap: 8px; }
            .btn-icon { font-size: 22px; }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header-row">
        <div class="header-controls">
            <button class="btn-icon" onclick="toggleList()" title="Danh sách từ">☰</button>
            <button class="btn-icon" onclick="toggleStats()" title="Thống kê">📊</button>
            <button class="btn-icon" onclick="toggleSettings()" title="Cài đặt âm thanh">⚙️</button>
            <button class="btn-icon" onclick="shuffleVocabulary()" title="Đảo thứ tự">🔀</button>
        </div>
        <div id="progress" class="progress-bar">CÂU 1 / 100</div>
    </div>

    <!-- Status Badge -->
    <div id="current-status" class="status-badge status-new">Mới</div>
    
    <div class="card">
        <!-- Phần câu hỏi Tiếng Việt -->
        <div id="question-area">
            <div class="vietnamese-text" id="vn-text">Đang tải dữ liệu...</div>
        </div>

        <!-- Phần đáp án (Ẩn) -->
        <div id="answer-area" class="hidden-content">
            <div class="part-of-speech" id="pos-text"></div>
            
            <!-- Hàng chứa từ và loa -->
            <div class="english-row">
                <div class="english-word" id="en-text"></div>
                <button class="btn-audio-replay" onclick="playCurrentAudio()" title="Nghe lại">🔊</button>
            </div>
            
            <!-- Phiên âm IPA -->
            <div class="ipa-text" id="ipa-text"></div>

            <!-- FIX: Thêm lại div example-text để hiển thị ví dụ -->
            <div class="example-box" id="example-text"></div>
        </div>
    </div>

    <div id="status-msg" class="status-msg"></div>

    <!-- Nút điều khiển chính -->
    <div id="main-actions">
        <button id="btn-reveal" class="btn btn-reveal" onclick="revealAnswer()">XEM ĐÁP ÁN</button>
    </div>

    <!-- Nút Đánh dấu (Hiện sau khi xem đáp án) -->
    <div id="review-actions" class="review-actions" style="display: none;">
        <button class="btn btn-learn" onclick="markStatus('learning')">Chưa thuộc 😕</button>
        <button class="btn btn-success" onclick="markStatus('learned')">Đã thuộc 😎</button>
    </div>

    <!-- Thanh điều hướng -->
    <div class="nav-row">
        <button class="btn btn-nav" onclick="changeCard(-1)">❮</button>
        <button class="btn btn-nav" onclick="changeCard(1)">❯</button>
    </div>
</div>

<!-- Modal Danh Sách -->
<div id="list-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Danh Sách 100 Từ</h3>
            <button onclick="toggleList()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        <div class="list-container" id="vocab-list-content"></div>
    </div>
</div>

<!-- Modal Thống Kê -->
<div id="stats-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Thống Kê Học Tập</h3>
            <button onclick="toggleStats()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        
        <div class="stats-summary">
            <div class="stat-box bg-learned">
                <span class="stat-val" id="stat-learned">0</span>
                <span class="stat-label">Đã thuộc</span>
            </div>
            <div class="stat-box bg-learning">
                <span class="stat-val" id="stat-learning">0</span>
                <span class="stat-label">Chưa thuộc</span>
            </div>
            <div class="stat-box bg-new">
                <span class="stat-val" id="stat-new">0</span>
                <span class="stat-label">Mới</span>
            </div>
        </div>

        <hr style="border:0; border-top:1px solid #eee; width:100%; margin: 10px 0;">
        <h4 style="margin: 0 0 10px 0; color: #555;">💡 Từ cần học ngay:</h4>
        <div class="recommend-section" id="recommend-list"></div>
    </div>
</div>

<!-- Modal Cài Đặt -->
<div id="settings-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Cài Đặt Âm Thanh</h3>
            <button onclick="toggleSettings()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        
        <div style="padding: 10px 0;">
            <div class="settings-row">
                <label class="settings-label">Chọn Giọng Đọc:</label>
                <select id="voice-select" class="settings-input" onchange="updateVoiceSettings()">
                    <option value="-1">Đang tải danh sách giọng...</option>
                </select>
            </div>
            
            <div class="settings-row">
                <label class="settings-label">Tốc Độ Đọc: <span id="speed-display" style="color:var(--primary-color)">0.7</span></label>
                <input type="range" id="speed-range" min="0.5" max="1.5" step="0.1" value="0.7" oninput="updateSpeedSettings()">
                <div style="display:flex; justify-content:space-between; font-size:12px; color:#999; margin-top:5px;">
                    <span>Chậm (0.5)</span>
                    <span>Nhanh (1.5)</span>
                </div>
            </div>
            
            <button class="btn" style="width:100%; margin-top:10px;" onclick="testVoice()">🔊 Nghe thử</button>
        </div>
    </div>
</div>

<script>
    // === DỮ LIỆU TỪ VỰNG 100 CÂU ===
    const initialVocabulary = [
        // --- 1. WORK & STUDY ---
        { en: "Major in", vi: "Chuyên ngành về...", ipa: "/ˈmeɪdʒər ɪn/", pos: "Verb Phrase", ex: "I decided to major in Marketing to understand consumer behavior." },
        { en: "Prestigious university", vi: "Trường đại học danh tiếng", ipa: "/prɛˈstɪdʒəs ˌjuːnɪˈvɜːrsəti/", pos: "Noun Phrase", ex: "Graduating from a prestigious university can open many doors." },
        { en: "Pursue a career in", vi: "Theo đuổi sự nghiệp trong lĩnh vực...", ipa: "/pərˈsuː ə kəˈrɪər ɪn/", pos: "Verb Phrase", ex: "She wants to pursue a career in digital journalism." },
        { en: "Land a job", vi: "Kiếm được công việc", ipa: "/lænd ə dʒɒb/", pos: "Verb Phrase", ex: "He managed to land a job at Google right after graduation." },
        { en: "9-to-5 job", vi: "Công việc hành chính", ipa: "/ˌnaɪn.təˈfaɪv dʒɒb/", pos: "Noun Phrase", ex: "I prefer a stable 9-to-5 job over freelancing." },
        { en: "Full-time / Part-time", vi: "Toàn thời gian / Bán thời gian", ipa: "/ˌfʊlˈtaɪm / ˌpɑːrtˈtaɪm/", pos: "Adjective", ex: "Students often find part-time jobs to cover their living expenses." },
        { en: "Work environment", vi: "Môi trường làm việc", ipa: "/wɜːrk ɪnˈvaɪrənmənt/", pos: "Noun Phrase", ex: "A toxic work environment significantly affects employee productivity." },
        { en: "Colleagues / Coworkers", vi: "Đồng nghiệp", ipa: "/ˈkɒliːɡz / ˈkoʊˌwɜːrkərz/", pos: "Noun", ex: "My colleagues are very friendly and always willing to help." },
        { en: "Supportive", vi: "Hỗ trợ, giúp đỡ nhau", ipa: "/səˈpɔːrtɪv/", pos: "Adjective", ex: "The teachers at this school are very supportive of their students." },
        { en: "State-of-the-art facilities", vi: "Cơ sở vật chất hiện đại", ipa: "/ˌsteɪt.əv.ðiˈɑːrt fəˈsɪlətiz/", pos: "Noun Phrase", ex: "The research lab is equipped with state-of-the-art facilities." },
        { en: "Heavy workload", vi: "Khối lượng công việc lớn", ipa: "/ˈhɛvi ˈwɜːrkloʊd/", pos: "Noun Phrase", ex: "I am dealing with a heavy workload this quarter." },
        { en: "Meet a deadline", vi: "Kịp hạn chót", ipa: "/miːt ə ˈdɛdlaɪn/", pos: "Verb Phrase", ex: "We must work overtime to meet the deadline." },
        { en: "Work under pressure", vi: "Làm việc dưới áp lực", ipa: "/wɜːrk ˈʌndər ˈprɛʃər/", pos: "Verb Phrase", ex: "Being able to work under pressure is a required skill for this job." },
        { en: "Hectic schedule", vi: "Lịch trình bận rộn", ipa: "/ˈhɛktɪk ˈʃɛdjuːl/", pos: "Noun Phrase", ex: "Despite his hectic schedule, he always finds time for his family." },
        { en: "Up to my ears in work", vi: "Bận ngập đầu", ipa: "/ʌp tu maɪ ɪərz ɪn wɜːrk/", pos: "Idiom", ex: "I can't go out tonight, I'm up to my ears in work." },
        { en: "Burn the midnight oil", vi: "Thức khuya làm việc/học bài", ipa: "/bɜːrn ðə ˈmɪdnaɪt ɔɪl/", pos: "Idiom", ex: "She burnt the midnight oil to finish her thesis." },
        { en: "Pass with flying colors", vi: "Đậu điểm cao", ipa: "/pæs wɪð ˈflaɪɪŋ ˈkʌlərz/", pos: "Idiom", ex: "He prepared well and passed the exam with flying colors." },
        { en: "Challenging but rewarding", vi: "Thử thách nhưng xứng đáng", ipa: "/ˈtʃælɪndʒɪŋ bʌt rɪˈwɔːrdɪŋ/", pos: "Adjective Phrase", ex: "Teaching children is challenging but rewarding." },
        { en: "Broaden my horizons", vi: "Mở rộng tầm mắt/kiến thức", ipa: "/ˈbrɔːdn maɪ həˈraɪzənz/", pos: "Verb Phrase", ex: "Traveling to new countries helps broaden my horizons." },
        { en: "Practical experience", vi: "Kinh nghiệm thực tế", ipa: "/ˈpræktɪkl ɪkˈspɪəriəns/", pos: "Noun Phrase", ex: "Internships provide students with valuable practical experience." },
        { en: "Lucrative income", vi: "Thu nhập cao/hậu hĩnh", ipa: "/ˈluːkrətɪv ˈɪnkʌm/", pos: "Noun Phrase", ex: "The IT industry offers a very lucrative income." },
        { en: "Make a living", vi: "Kiếm sống", ipa: "/meɪk ə ˈlɪvɪŋ/", pos: "Verb Phrase", ex: "It's becoming harder to make a living as an artist." },
        { en: "Cover my bills", vi: "Trang trải chi phí sinh hoạt", ipa: "/ˈkʌvər maɪ bɪlz/", pos: "Verb Phrase", ex: "I need a second job to cover my bills." },
        { en: "Promotion opportunities", vi: "Cơ hội thăng tiến", ipa: "/prəˈmoʊʃn ˌɒpərˈtuːnətiz/", pos: "Noun Phrase", ex: "This company offers great promotion opportunities for hard workers." },
        { en: "Get promoted", vi: "Được thăng chức", ipa: "/ɡɛt prəˈmoʊtɪd/", pos: "Verb Phrase", ex: "She got promoted to Senior Manager last month." },
        { en: "Soft skills", vi: "Kỹ năng mềm", ipa: "/sɒft skɪlz/", pos: "Noun Phrase", ex: "Communication and teamwork are essential soft skills." },
        { en: "Teamwork spirit", vi: "Tinh thần đồng đội", ipa: "/ˈtiːmwɜːrk ˈspɪrɪt/", pos: "Noun Phrase", ex: "The manager values strong teamwork spirit in the office." },
        { en: "Job satisfaction", vi: "Sự hài lòng trong công việc", ipa: "/dʒɒb ˌsætɪsˈfækʃn/", pos: "Noun Phrase", ex: "For me, job satisfaction is more important than a high salary." },
        { en: "Stable job", vi: "Công việc ổn định", ipa: "/ˈsteɪbl dʒɒb/", pos: "Noun Phrase", ex: "My parents want me to have a stable job in the government." },
        { en: "Gap year", vi: "Năm nghỉ phép để trải nghiệm", ipa: "/ɡæp jɪər/", pos: "Noun", ex: "I took a gap year to travel across Europe before starting university." },

        // --- 2. HOMETOWN ---
        { en: "Located in / Situated in", vi: "Nằm ở...", ipa: "/loʊˈkeɪtɪd ɪn / ˈsɪtʃueɪtɪd ɪn/", pos: "Verb Phrase", ex: "My hometown is situated in the coastal region of Vietnam." },
        { en: "Coastal city", vi: "Thành phố biển", ipa: "/ˈkoʊstl ˈsɪti/", pos: "Noun Phrase", ex: "Da Nang is a beautiful coastal city famous for its beaches." },
        { en: "Mountainous area", vi: "Khu vực miền núi", ipa: "/ˈmaʊntənəs ˈeriə/", pos: "Noun Phrase", ex: "Living in a mountainous area offers fresh air but travel can be difficult." },
        { en: "The suburbs / Outskirts", vi: "Vùng ngoại ô", ipa: "/ðə ˈsʌbɜːrbz / ˈaʊtskɜːrts/", pos: "Noun", ex: "I live in the suburbs, so it takes me 30 minutes to drive to the city center." },
        { en: "Heart of the city", vi: "Trung tâm thành phố", ipa: "/hɑːrt əv ðə ˈsɪti/", pos: "Noun Phrase", ex: "My apartment is right in the heart of the city." },
        { en: "Industrial zone", vi: "Khu công nghiệp", ipa: "/ɪnˈdʌstriəl zoʊn/", pos: "Noun Phrase", ex: "There is a large industrial zone near my town providing jobs for locals." },
        { en: "Tourist attraction", vi: "Điểm thu hút du lịch", ipa: "/ˈtʊərɪst əˈtrækʃn/", pos: "Noun Phrase", ex: "Ha Long Bay is a major tourist attraction in Vietnam." },
        { en: "Picturesque landscapes", vi: "Phong cảnh đẹp như tranh", ipa: "/ˌpɪktʃəˈrɛsk ˈlændskeɪps/", pos: "Noun Phrase", ex: "Sapa is known for its picturesque landscapes and terraced rice fields." },
        { en: "Breathtaking view", vi: "Cảnh đẹp nín thở", ipa: "/ˈbrɛθteɪkɪŋ vjuː/", pos: "Noun Phrase", ex: "The hotel room offers a breathtaking view of the ocean." },
        { en: "Historical sites", vi: "Di tích lịch sử", ipa: "/hɪˈstɔːrɪkl saɪts/", pos: "Noun Phrase", ex: "Hue is famous for its many historical sites and ancient tombs." },
        { en: "Pace of life", vi: "Nhịp sống", ipa: "/peɪs əv laɪf/", pos: "Noun Phrase", ex: "The pace of life in the countryside is much slower than in the city." },
        { en: "Hustle and bustle", vi: "Sự hối hả nhộn nhịp", ipa: "/ˈhʌsl ənd ˈbʌsl/", pos: "Idiom/Noun", ex: "I enjoy the hustle and bustle of city life." },
        { en: "Tranquil / Peaceful", vi: "Yên bình", ipa: "/ˈtræŋkwɪl / ˈpiːsfl/", pos: "Adjective", ex: "I love the tranquil atmosphere of my village." },
        { en: "Fresh air", vi: "Không khí trong lành", ipa: "/frɛʃ ɛər/", pos: "Noun Phrase", ex: "We went to the park to breathe some fresh air." },
        { en: "Polluted", vi: "Ô nhiễm", ipa: "/pəˈluːtɪd/", pos: "Adjective", ex: "The air in big cities is becoming heavily polluted." },
        { en: "Traffic congestion", vi: "Tắc đường", ipa: "/ˈtræfɪk kənˈdʒɛstʃən/", pos: "Noun Phrase", ex: "Traffic congestion is a serious problem during rush hour." },
        { en: "Commute", vi: "Việc đi lại (từ nhà đến chỗ làm)", ipa: "/kəˈmjuːt/", pos: "Noun/Verb", ex: "My daily commute takes about 45 minutes by bus." },
        { en: "Crowded / Packed", vi: "Đông đúc", ipa: "/ˈkraʊdɪd / pækt/", pos: "Adjective", ex: "The streets are always crowded during festivals." },
        { en: "Vibrant", vi: "Sôi động, đầy sức sống", ipa: "/ˈvaɪbrənt/", pos: "Adjective", ex: "Ho Chi Minh City has a vibrant nightlife." },
        { en: "Dull / Boring", vi: "Nhàm chán", ipa: "/dʌl / ˈbɔːrɪŋ/", pos: "Adjective", ex: "Some people find life in the countryside a bit dull." },
        { en: "Hospitable", vi: "Hiếu khách", ipa: "/hɒˈspɪtəbl/", pos: "Adjective", ex: "The local people are incredibly hospitable to tourists." },
        { en: "Friendly and welcoming", vi: "Thân thiện và chào đón", ipa: "/ˈfrɛndli ənd ˈwɛlkəmɪŋ/", pos: "Adjective Phrase", ex: "My neighbors are very friendly and welcoming." },
        { en: "Sense of community", vi: "Tinh thần cộng đồng", ipa: "/sɛns əv kəˈmjuːnəti/", pos: "Noun Phrase", ex: "There is a strong sense of community in this small town." },
        { en: "Local delicacies", vi: "Đặc sản địa phương", ipa: "/ˈloʊkl ˈdɛlɪkəsiz/", pos: "Noun Phrase", ex: "You must try the local delicacies when you visit Hanoi." },
        { en: "Street food", vi: "Đồ ăn đường phố", ipa: "/striːt fuːd/", pos: "Noun Phrase", ex: "Vietnam is famous for its delicious and cheap street food." },
        { en: "Amenities", vi: "Các tiện ích", ipa: "/əˈmiːnətiz/", pos: "Noun", ex: "The apartment complex has excellent amenities like a pool and gym." },
        { en: "Entertainment centers", vi: "Khu vui chơi giải trí", ipa: "/ˌɛntərˈteɪnmənt ˈsɛntərz/", pos: "Noun Phrase", ex: "Young people often hang out at entertainment centers on weekends." },
        { en: "Public transport system", vi: "Hệ thống giao thông công cộng", ipa: "/ˈpʌblɪk ˈtrænspɔːrt ˈsɪstəm/", pos: "Noun Phrase", ex: "The city needs to improve its public transport system." },
        { en: "Shopping mall", vi: "Trung tâm thương mại", ipa: "/ˈʃɒpɪŋ mɔːl/", pos: "Noun Phrase", ex: "We spent the whole afternoon at the shopping mall." },
        { en: "Undergo dramatic changes", vi: "Trải qua thay đổi mạnh mẽ", ipa: "/ˌʌndərˈɡoʊ drəˈmætɪk ˈtʃeɪndʒɪz/", pos: "Verb Phrase", ex: "My hometown has undergone dramatic changes in the last decade." },

        // --- 3. ACCOMMODATION ---
        { en: "Apartment block / Flat", vi: "Chung cư/Căn hộ", ipa: "/əˈpɑːrtmənt blɒk / flæt/", pos: "Noun", ex: "I live in a modern apartment block near the river." },
        { en: "Terraced house", vi: "Nhà phố (liền kề)", ipa: "/ˈtɛrəst haʊs/", pos: "Noun", ex: "Terraced houses are very common in the UK." },
        { en: "Detached house", vi: "Nhà riêng biệt lập", ipa: "/dɪˈtætʃt haʊs/", pos: "Noun", ex: "A detached house offers more privacy than an apartment." },
        { en: "Dormitory", vi: "Ký túc xá", ipa: "/ˈdɔːrmətɔːri/", pos: "Noun", ex: "Living in a dormitory is a great way to make friends at college." },
        { en: "Rented accommodation", vi: "Nhà thuê", ipa: "/ˈrɛntɪd əˌkɒməˈdeɪʃn/", pos: "Noun Phrase", ex: "Students usually live in rented accommodation." },
        { en: "Residential area", vi: "Khu dân cư", ipa: "/ˌrɛzɪˈdɛnʃl ˈeriə/", pos: "Noun Phrase", ex: "My house is in a quiet residential area." },
        { en: "Convenient location", vi: "Vị trí thuận tiện", ipa: "/kənˈviːniənt loʊˈkeɪʃn/", pos: "Noun Phrase", ex: "The hotel has a convenient location near the subway station." },
        { en: "Within walking distance of", vi: "Gần (có thể đi bộ tới)", ipa: "/wɪˈðɪn ˈwɔːkɪŋ ˈdɪstəns əv/", pos: "Prepositional Phrase", ex: "My office is within walking distance of my house." },
        { en: "Prime location", vi: "Vị trí đắc địa", ipa: "/praɪm loʊˈkeɪʃn/", pos: "Noun Phrase", ex: "The shop is in a prime location on the main street." },
        { en: "Overlook", vi: "Nhìn ra (công viên/hồ)", ipa: "/ˌoʊvərˈlʊk/", pos: "Verb", ex: "My bedroom window overlooks a beautiful park." },
        { en: "Spacious", vi: "Rộng rãi", ipa: "/ˈspeɪʃəs/", pos: "Adjective", ex: "The living room is very spacious and bright." },
        { en: "Cramped", vi: "Chật chội", ipa: "/kræmpt/", pos: "Adjective", ex: "The apartment is a bit cramped for a family of four." },
        { en: "Cozy", vi: "Ấm cúng", ipa: "/ˈkoʊzi/", pos: "Adjective", ex: "I love my small, cozy bedroom." },
        { en: "Airy", vi: "Thoáng khí", ipa: "/ˈeri/", pos: "Adjective", ex: "With large windows, the room feels very airy." },
        { en: "Stuffy", vi: "Bí bách", ipa: "/ˈstʌfi/", pos: "Adjective", ex: "It gets very stuffy in here during the summer." },
        { en: "Fully furnished", vi: "Đầy đủ nội thất", ipa: "/ˈfʊli ˈfɜːrnɪʃt/", pos: "Adjective", ex: "I rented a fully furnished apartment to save money on furniture." },
        { en: "Modern appliances", vi: "Thiết bị hiện đại", ipa: "/ˈmɒdərn əˈplaɪənsɪz/", pos: "Noun Phrase", ex: "The kitchen is equipped with modern appliances." },
        { en: "Decorate", vi: "Trang trí", ipa: "/ˈdɛkəreɪt/", pos: "Verb", ex: "I like to decorate my room with plants and paintings." },
        { en: "Renovate", vi: "Sửa sang, nâng cấp", ipa: "/ˈrɛnəveɪt/", pos: "Verb", ex: "We plan to renovate the bathroom next year." },
        { en: "Balcony", vi: "Ban công", ipa: "/ˈbælkəni/", pos: "Noun", ex: "I often drink coffee on the balcony in the morning." },
        { en: "House chores", vi: "Việc nhà", ipa: "/haʊs tʃɔːrz/", pos: "Noun", ex: "My brother and I share the house chores." },
        { en: "Do the laundry", vi: "Giặt đồ", ipa: "/duː ðə ˈlɔːndri/", pos: "Verb Phrase", ex: "I usually do the laundry on Sundays." },
        { en: "Tidy up", vi: "Dọn dẹp", ipa: "/ˈtaɪdi ʌp/", pos: "Verb Phrase", ex: "Please tidy up your room before guests arrive." },
        { en: "Family gathering", vi: "Tụ họp gia đình", ipa: "/ˈfæməli ˈɡæðərɪŋ/", pos: "Noun Phrase", ex: "We have a family gathering every Lunar New Year." },
        { en: "Privacy", vi: "Sự riêng tư", ipa: "/ˈprɪvəsi/", pos: "Noun", ex: "Everyone needs some privacy now and then." },
        { en: "Unwind / Chill out", vi: "Thư giãn", ipa: "/ˌʌnˈwaɪnd / tʃɪl aʊt/", pos: "Verb", ex: "Listening to music helps me unwind after work." },
        { en: "Housewarming party", vi: "Tiệc tân gia", ipa: "/ˈhaʊswɔːrmɪŋ ˈpɑːrti/", pos: "Noun Phrase", ex: "They invited us to their housewarming party." },
        { en: "Get on well with neighbors", vi: "Hòa thuận với hàng xóm", ipa: "/ɡɛt ɒn wɛl wɪð ˈneɪbərz/", pos: "Verb Phrase", ex: "Luckily, we get on very well with our neighbors." },
        { en: "Noisy neighbors", vi: "Hàng xóm ồn ào", ipa: "/ˈnɔɪzi ˈneɪbərz/", pos: "Noun Phrase", ex: "Having noisy neighbors can be really annoying." },
        { en: "Feel at home", vi: "Cảm thấy thoải mái như ở nhà", ipa: "/fiːl æt hoʊm/", pos: "Idiom", ex: "Please sit down and feel at home." },

        // --- 4. LINKING WORDS ---
        { en: "Actually / To be honest", vi: "Thật ra thì / Thành thật mà nói", ipa: "/ˈæktʃuəli / tuː bi ˈɒnɪst/", pos: "Adverb/Phrase", ex: "Actually, I haven't finished the report yet." },
        { en: "Generally speaking", vi: "Nói chung là", ipa: "/ˈdʒɛnərəli ˈspiːkɪŋ/", pos: "Phrase", ex: "Generally speaking, the weather here is quite nice." },
        { en: "What I like most about X is", vi: "Điều tôi thích nhất ở X là...", ipa: "/wɒt aɪ laɪk moʊst əˈbaʊt ... ɪz/", pos: "Phrase", ex: "What I like most about this job is the flexibility." },
        { en: "I’m really keen on", vi: "Tôi rất thích...", ipa: "/aɪm ˈrɪəli kiːn ɒn/", pos: "Phrase", ex: "I’m really keen on playing football." },
        { en: "It allows me to", vi: "Nó cho phép tôi làm gì...", ipa: "/ɪt əˈlaʊz miː tuː/", pos: "Phrase", ex: "This software allows me to work much faster." },
        { en: "Once in a blue moon", vi: "Hiếm khi", ipa: "/wʌns ɪn ə bluː muːn/", pos: "Idiom", ex: "I go to the cinema once in a blue moon." },
        { en: "Day in, day out", vi: "Ngày qua ngày", ipa: "/deɪ ɪn, deɪ aʊt/", pos: "Idiom", ex: "He does the same boring job day in, day out." },
        { en: "For the most part", vi: "Phần lớn là", ipa: "/fɔːr ðə moʊst pɑːrt/", pos: "Phrase", ex: "For the most part, I agree with your opinion." },
        { en: "On top of that", vi: "Thêm vào đó", ipa: "/ɒn tɒp əv ðæt/", pos: "Phrase", ex: "The job is interesting, and on top of that, the pay is good." },
        { en: "Last but not least", vi: "Cuối cùng nhưng không kém phần quan trọng", ipa: "/læst bʌt nɒt liːst/", pos: "Phrase", ex: "And last but not least, I'd like to thank my parents." }
    ];

    let vocabularyList = initialVocabulary.map(item => ({...item, status: 'new'}));
    
    let currentIndex = 0;
    let isRevealed = false;
    let availableVoices = [];
    
    // Global settings for audio
    let selectedVoiceIndex = -1; // -1 means auto-detect
    let readingRate = 0.7; // Default slow speed

    // Elements
    const elements = {
        vnText: document.getElementById('vn-text'),
        enText: document.getElementById('en-text'),
        ipaText: document.getElementById('ipa-text'), // New element for IPA
        posText: document.getElementById('pos-text'),
        exText: document.getElementById('example-text'),
        answerArea: document.getElementById('answer-area'),
        btnReveal: document.getElementById('btn-reveal'),
        reviewActions: document.getElementById('review-actions'),
        statusMsg: document.getElementById('status-msg'),
        progress: document.getElementById('progress'),
        currentStatus: document.getElementById('current-status'),
        listModal: document.getElementById('list-modal'),
        listContent: document.getElementById('vocab-list-content'),
        statsModal: document.getElementById('stats-modal'),
        statLearned: document.getElementById('stat-learned'),
        statLearning: document.getElementById('stat-learning'),
        statNew: document.getElementById('stat-new'),
        recommendList: document.getElementById('recommend-list'),
        settingsModal: document.getElementById('settings-modal'),
        voiceSelect: document.getElementById('voice-select'),
        speedRange: document.getElementById('speed-range'),
        speedDisplay: document.getElementById('speed-display')
    };

    // === SETUP AUDIO (PURE SYSTEM SPEECH) ===
    function loadVoices() {
        availableVoices = window.speechSynthesis.getVoices();
        
        // Populate Dropdown
        elements.voiceSelect.innerHTML = '';
        
        // Option Mặc định
        const defaultOption = document.createElement('option');
        defaultOption.value = -1;
        defaultOption.text = "Tự động chọn (Tốt nhất)";
        elements.voiceSelect.appendChild(defaultOption);

        availableVoices.forEach((voice, index) => {
            // Chỉ hiện các giọng có tiếng Anh để đỡ rối
            if(voice.lang.includes('en')) {
                const option = document.createElement('option');
                option.value = index;
                option.text = `${voice.name} (${voice.lang})`;
                // Đánh dấu nếu đang được chọn
                if (index === selectedVoiceIndex) option.selected = true;
                elements.voiceSelect.appendChild(option);
            }
        });
    }
    
    if (speechSynthesis.onvoiceschanged !== undefined) {
        speechSynthesis.onvoiceschanged = loadVoices;
    }
    // Gọi lần đầu (đôi khi trình duyệt đã load xong rồi)
    setTimeout(loadVoices, 100);

    function playAudio(text) {
        window.speechSynthesis.cancel();
        const utterance = new SpeechSynthesisUtterance(text);
        
        // Xác định giọng đọc
        if (selectedVoiceIndex !== -1 && availableVoices[selectedVoiceIndex]) {
            // Người dùng đã chọn giọng cụ thể
            utterance.voice = availableVoices[selectedVoiceIndex];
        } else {
            // Tự động chọn (Ưu tiên Google / Premium / UK)
            let preferredVoice = availableVoices.find(voice => 
                (voice.name.includes('Google') && voice.lang.includes('en')) || 
                (voice.name.includes('Premium') && voice.lang.includes('en')) ||
                (voice.name.includes('Samantha') && voice.lang.includes('en'))
            );

            if (!preferredVoice) {
                preferredVoice = availableVoices.find(voice => voice.lang === 'en-GB' || voice.lang === 'en_GB');
            }
            if (!preferredVoice) {
                preferredVoice = availableVoices.find(voice => voice.lang.includes('en'));
            }

            if (preferredVoice) utterance.voice = preferredVoice;
        }
        
        // Áp dụng tốc độ
        utterance.rate = readingRate; 
        utterance.pitch = 1.0;
        utterance.volume = 1.0;

        utterance.onerror = (e) => console.log('Speech error:', e);
        window.speechSynthesis.speak(utterance);
    }

    // --- SETTINGS FUNCTIONS ---
    function toggleSettings() {
        const isHidden = elements.settingsModal.style.display === 'none' || elements.settingsModal.style.display === '';
        if (isHidden) {
            elements.settingsModal.style.display = 'flex';
            // Refresh voice list in case it wasn't loaded
            if(availableVoices.length === 0) loadVoices();
        } else {
            elements.settingsModal.style.display = 'none';
        }
    }

    function updateVoiceSettings() {
        selectedVoiceIndex = parseInt(elements.voiceSelect.value);
        // Lưu ý: Không cần lưu localStorage vì đề bài không yêu cầu, 
        // nhưng biến selectedVoiceIndex là toàn cục nên sẽ áp dụng cho mọi từ.
    }

    function updateSpeedSettings() {
        readingRate = parseFloat(elements.speedRange.value);
        elements.speedDisplay.innerText = readingRate;
    }
    
    function testVoice() {
        playAudio("Hello, this is a test for English voice.");
    }

    // --- OTHER LOGIC ---
    function shuffleVocabulary() {
        for (let i = vocabularyList.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1));
            [vocabularyList[i], vocabularyList[j]] = [vocabularyList[j], vocabularyList[i]];
        }
        currentIndex = 0;
        loadCard(0);
        elements.statusMsg.innerText = "🔀 Đã đảo thứ tự từ vựng!";
        setTimeout(() => elements.statusMsg.innerText = "", 2000);
    }

    function loadCard(index) {
        if (index < 0) currentIndex = vocabularyList.length - 1;
        else if (index >= vocabularyList.length) currentIndex = 0;
        else currentIndex = index;

        const item = vocabularyList[currentIndex];

        elements.vnText.innerText = item.vi;
        elements.enText.innerText = item.en;
        elements.posText.innerText = item.pos;
        
        // FIX: Check if exText element exists and if item has example data
        if(elements.exText) {
             if(item.ex) {
                elements.exText.innerText = `Ví dụ: "${item.ex}"`;
                elements.exText.style.display = 'block';
            } else {
                elements.exText.style.display = 'none';
            }
        }
        
        // Cập nhật IPA
        if (item.ipa) {
            elements.ipaText.innerText = item.ipa;
            elements.ipaText.style.display = 'block';
        } else {
            elements.ipaText.style.display = 'none';
        }
        
        elements.answerArea.style.display = 'none';
        elements.reviewActions.style.display = 'none';
        elements.btnReveal.style.display = 'block';
        elements.btnReveal.disabled = false;
        elements.btnReveal.innerText = "XEM ĐÁP ÁN";
        elements.statusMsg.innerText = "";
        
        elements.progress.innerText = `CÂU ${currentIndex + 1} / ${vocabularyList.length}`;
        updateStatusBadge(item.status);
        
        isRevealed = false;
    }

    function updateStatusBadge(status) {
        elements.currentStatus.className = 'status-badge';
        if (status === 'learned') {
            elements.currentStatus.innerText = "Đã thuộc";
            elements.currentStatus.classList.add('status-learned');
        } else if (status === 'learning') {
            elements.currentStatus.innerText = "Chưa thuộc";
            elements.currentStatus.classList.add('status-learning');
        } else {
            elements.currentStatus.innerText = "Mới";
            elements.currentStatus.classList.add('status-new');
        }
    }

    function revealAnswer() {
        isRevealed = true;
        elements.btnReveal.disabled = true;
        elements.answerArea.style.display = 'block';
        playAudio(vocabularyList[currentIndex].en);
        elements.btnReveal.style.display = 'none'; 
        elements.reviewActions.style.display = 'flex'; 
    }

    function playCurrentAudio() {
        playAudio(vocabularyList[currentIndex].en);
    }

    function markStatus(status) {
        vocabularyList[currentIndex].status = status;
        updateStatusBadge(status);
        setTimeout(() => { changeCard(1); }, 300);
    }

    function changeCard(step) {
        loadCard(currentIndex + step);
    }

    function toggleList() {
        const isHidden = elements.listModal.style.display === 'none' || elements.listModal.style.display === '';
        if (isHidden) {
            renderList();
            elements.listModal.style.display = 'flex';
        } else {
            elements.listModal.style.display = 'none';
        }
    }

    function renderList() {
        elements.listContent.innerHTML = '';
        vocabularyList.forEach((item, index) => {
            const div = document.createElement('div');
            div.className = `list-item ${index === currentIndex ? 'active' : ''}`;
            let statusIcon = '⚪';
            if (item.status === 'learned') statusIcon = '✅';
            if (item.status === 'learning') statusIcon = '🔸';
            div.innerHTML = `<div style="display:flex; align-items:center;"><span style="margin-right:8px; font-size: 12px;">${statusIcon}</span><strong>${item.en}</strong></div><div style="font-size:12px; color:#666;">${index + 1}</div>`;
            div.onclick = () => { currentIndex = index; loadCard(currentIndex); toggleList(); };
            elements.listContent.appendChild(div);
        });
    }

    function toggleStats() {
        const isHidden = elements.statsModal.style.display === 'none' || elements.statsModal.style.display === '';
        if (isHidden) { renderStats(); elements.statsModal.style.display = 'flex'; } else { elements.statsModal.style.display = 'none'; }
    }

    function renderStats() {
        const learnedCount = vocabularyList.filter(i => i.status === 'learned').length;
        const learningCount = vocabularyList.filter(i => i.status === 'learning').length;
        const newCount = vocabularyList.filter(i => i.status === 'new').length;
        elements.statLearned.innerText = learnedCount;
        elements.statLearning.innerText = learningCount;
        elements.statNew.innerText = newCount;
        let recommendItems = vocabularyList.map((item, index) => ({ ...item, originalIndex: index })).filter(i => i.status === 'learning');
        elements.recommendList.innerHTML = '';
        if (recommendItems.length === 0) {
            const newItems = vocabularyList.map((item, index) => ({ ...item, originalIndex: index })).filter(i => i.status === 'new').slice(0, 5);
            if (newItems.length > 0) {
                elements.recommendList.innerHTML = '<div style="color:#777; font-style:italic; padding:10px;">Bạn đã thuộc hết các từ cần ôn. Hãy học từ mới:</div>';
                newItems.forEach(item => createRecommendItem(item));
            } else {
                elements.recommendList.innerHTML = '<div style="color:green; padding:10px; text-align:center;">🎉 Tuyệt vời! Bạn đã thuộc hết toàn bộ danh sách.</div>';
            }
        } else {
            recommendItems.forEach(item => createRecommendItem(item));
        }
    }

    function createRecommendItem(item) {
        const div = document.createElement('div');
        div.className = 'recommend-item';
        div.innerHTML = `🔸 <strong>${item.en}</strong> <span style="font-size:12px; color:#999;">(${item.vi})</span>`;
        div.onclick = () => { currentIndex = item.originalIndex; loadCard(currentIndex); toggleStats(); };
        elements.recommendList.appendChild(div);
    }

    loadCard(0);
</script>

</body>
</html>
