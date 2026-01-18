<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>120 Collocations - 6 Phần</title>
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
            padding: 25px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(211, 47, 47, 0.15);
            width: 100%;
            max-width: 500px;
            text-align: center;
            border-top: 5px solid var(--primary-color);
            position: relative;
            box-sizing: border-box;
        }

        /* Deck Selector Styling */
        .deck-selector-container {
            margin-bottom: 15px;
            text-align: left;
        }
        
        .deck-select {
            width: 100%;
            padding: 10px;
            border-radius: 10px;
            border: 2px solid var(--primary-color);
            background-color: white;
            color: var(--text-color);
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            outline: none;
        }

        /* Header & Progress */
        .header-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }

        .header-controls {
            display: flex;
            gap: 8px;
        }

        .btn-icon {
            background: none;
            border: none;
            font-size: 22px; 
            cursor: pointer;
            color: var(--primary-color);
            padding: 5px;
            transition: transform 0.2s;
            border-radius: 5px;
        }
        .btn-icon:hover { transform: scale(1.1); background-color: var(--accent-light); }
        .btn-icon.active { background-color: #ffcdd2; border: 1px solid var(--primary-color); }

        .progress-bar {
            color: #ef5350;
            font-weight: 600;
            font-size: 14px;
            letter-spacing: 1px;
        }

        /* Card Area - FIXED HEIGHT */
        .card {
            height: 420px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
            overflow-y: auto;
            padding: 10px;
            box-sizing: border-box;
            border: 1px solid #eee;
            border-radius: 15px;
            background: #fafafa;
        }
        
        .card::-webkit-scrollbar { width: 6px; }
        .card::-webkit-scrollbar-thumb { background-color: rgba(211, 47, 47, 0.2); border-radius: 4px; }

        .vietnamese-text {
            font-size: 22px;
            font-weight: bold;
            margin-bottom: 10px;
            color: #2c3e50;
            line-height: 1.4;
            word-wrap: break-word; 
        }
        
        .pos-tag {
            font-size: 14px; 
            color: #666; 
            margin-top: 5px; 
            font-weight: normal;
            font-style: italic;
            background: #eee;
            padding: 2px 8px;
            border-radius: 10px;
            display: inline-block;
        }

        .hidden-content {
            display: none;
            animation: fadeIn 0.5s ease-out;
            width: 100%;
        }

        .english-row {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin: 10px 0;
            flex-wrap: wrap;
        }

        .english-word {
            font-size: 28px;
            color: var(--primary-color);
            font-weight: 800;
            text-shadow: 1px 1px 0px rgba(0,0,0,0.05);
            margin: 0;
            word-break: break-word; 
        }

        .ipa-text {
            font-family: 'Lucida Sans Unicode', 'Arial Unicode MS', sans-serif;
            font-size: 16px;
            color: #757575;
            margin-bottom: 15px;
            font-weight: 400;
        }

        .btn-audio-replay {
            background: white;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
            width: 36px; 
            height: 36px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 18px;
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

        .example-box {
            font-size: 15px;
            color: #4b5563;
            margin-top: 10px;
            padding: 12px;
            background-color: #fff;
            border-left: 4px solid var(--primary-color);
            border-radius: 0 8px 8px 0;
            text-align: left;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            line-height: 1.5;
        }

        .btn {
            border: none;
            padding: 12px 20px; 
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

        .nav-row {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
            gap: 15px;
        }

        .btn-nav {
            background-color: white;
            color: var(--primary-color);
            border: 2px solid var(--primary-color);
            width: 50px; 
            height: 50px;
            border-radius: 50%;
            font-size: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0;
        }

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
            font-size: 12px;
            margin-top: 10px;
            color: #e53935;
            font-style: italic;
            height: 15px;
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
            .container { padding: 15px; }
            .vietnamese-text { font-size: 20px; }
            .english-word { font-size: 24px; }
            .card { height: 400px; }
            .btn { font-size: 15px; padding: 12px; }
            .btn-nav { width: 45px; height: 45px; font-size: 18px; }
            .header-controls { gap: 5px; }
            .btn-icon { font-size: 20px; padding: 4px; }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

<div class="container">
    <!-- Deck Selector -->
    <div class="deck-selector-container">
        <select id="deck-select" class="deck-select" onchange="changeDeck()">
            <option value="0">Phần 1: Từ 1 - 20</option>
            <option value="1">Phần 2: Từ 21 - 40</option>
            <option value="2">Phần 3: Từ 41 - 60</option>
            <option value="3">Phần 4: Từ 61 - 80</option>
            <option value="4">Phần 5: Từ 81 - 100</option>
            <option value="5">Phần 6: Từ 101 - 120</option>
        </select>
    </div>

    <div class="header-row">
        <div class="header-controls">
            <button class="btn-icon" onclick="toggleList()" title="Danh sách từ">☰</button>
            <button class="btn-icon" onclick="toggleStats()" title="Thống kê">📊</button>
            <button class="btn-icon" onclick="toggleSettings()" title="Cài đặt âm thanh">⚙️</button>
            <button class="btn-icon" id="btn-review" onclick="toggleReviewMode()" title="Ôn tập từ chưa thuộc">🧠</button>
            <button class="btn-icon" onclick="shuffleVocabulary()" title="Đảo thứ tự">🔀</button>
        </div>
        <div id="progress" class="progress-bar">CÂU 1 / 20</div>
    </div>

    <!-- Status Badge -->
    <div id="current-status" class="status-badge status-new">Mới</div>
    
    <div class="card">
        <!-- Phần câu hỏi Tiếng Việt -->
        <div id="question-area">
            <div class="vietnamese-text" id="vn-text"></div>
        </div>

        <!-- Phần đáp án (Ẩn) -->
        <div id="answer-area" class="hidden-content">
            <!-- Hàng chứa từ và loa -->
            <div class="english-row">
                <div class="english-word" id="en-text"></div>
                <button class="btn-audio-replay" onclick="playCurrentAudio()" title="Nghe lại">🔊</button>
            </div>
            
            <!-- Phiên âm IPA -->
            <div class="ipa-text" id="ipa-text"></div>

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
            <h3 style="margin:0; color:var(--primary-color)" id="list-title">Danh Sách</h3>
            <button onclick="toggleList()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        <div class="list-container" id="vocab-list-content"></div>
    </div>
</div>

<!-- Modal Thống Kê -->
<div id="stats-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Thống Kê (Phần Hiện Tại)</h3>
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
    // === DỮ LIỆU TỔNG HỢP 120 TỪ ===
    const allVocabulary = [
        // PART 1 (1-50)
        { en: "Major in [Subject]", vi: "Chuyên ngành về...", ipa: "/ˈmeɪ.dʒər ɪn/", pos: "v. phrase", ex: "I decided to major in Marketing." },
        { en: "Prestigious university", vi: "Trường đại học danh tiếng", ipa: "/presˈtɪdʒ.əs ˌjuː.nɪˈvɜː.sə.ti/", pos: "n. phrase", ex: "He graduated from a prestigious university." },
        { en: "Pursue a career in", vi: "Theo đuổi sự nghiệp trong lĩnh vực...", ipa: "/pəˈsjuː ə kəˈrɪər ɪn/", pos: "v. phrase", ex: "She wants to pursue a career in medicine." },
        { en: "Land a job", vi: "Kiếm được công việc", ipa: "/lænd ə dʒɒb/", pos: "v. phrase", ex: "He managed to land a job at Google." },
        { en: "9-to-5 job", vi: "Công việc hành chính", ipa: "/ˌnaɪn.təˈfaɪv dʒɒb/", pos: "n. phrase", ex: "I prefer a stable 9-to-5 job." },
        { en: "Full-time / Part-time", vi: "Toàn thời gian / Bán thời gian", ipa: "/ˌfʊlˈtaɪm/ - /ˌpɑːtˈtaɪm/", pos: "adj/adv", ex: "Students often work part-time." },
        { en: "Work environment", vi: "Môi trường làm việc", ipa: "/ˈwɜːk ɪnˌvaɪ.rən.mənt/", pos: "n. phrase", ex: "A good work environment is important." },
        { en: "Colleague / Coworker", vi: "Đồng nghiệp", ipa: "/ˈkɒl.iːɡ/ - /ˌkəʊˈwɜː.kər/", pos: "n", ex: "My colleagues are very friendly." },
        { en: "Supportive", vi: "Hỗ trợ, giúp đỡ nhau", ipa: "/səˈpɔː.tɪv/", pos: "adj", ex: "The team is very supportive." },
        { en: "State-of-the-art facilities", vi: "Cơ sở vật chất hiện đại", ipa: "/ˌsteɪt.əv.ðiˈɑːt fəˈsɪl.ə.tiz/", pos: "n. phrase", ex: "The lab has state-of-the-art facilities." },
        { en: "Heavy workload", vi: "Khối lượng công việc lớn", ipa: "/ˈhev.i ˈwɜːk.ləʊd/", pos: "n. phrase", ex: "I have a heavy workload this week." },
        { en: "Meet a deadline", vi: "Kịp hạn chót", ipa: "/miːt ə ˈded.laɪn/", pos: "v. phrase", ex: "We must work hard to meet the deadline." },
        { en: "Work under pressure", vi: "Làm việc dưới áp lực", ipa: "/wɜːk ˈʌn.dər ˈpreʃ.ər/", pos: "v. phrase", ex: "Can you work under pressure?" },
        { en: "Hectic schedule", vi: "Lịch trình bận rộn", ipa: "/ˈhek.tɪk ˈʃedʒ.uːl/", pos: "n. phrase", ex: "Despite his hectic schedule, he exercises daily." },
        { en: "Up to my ears in work", vi: "Bận ngập đầu", ipa: "/ʌp tu maɪ ɪəz ɪn wɜːk/", pos: "idiom", ex: "I'm up to my ears in work right now." },
        { en: "Burn the midnight oil", vi: "Thức khuya làm việc/học bài", ipa: "/bɜːn ðə ˈmɪd.naɪt ɔɪl/", pos: "idiom", ex: "She burnt the midnight oil to finish the essay." },
        { en: "Pass with flying colors", vi: "Đậu điểm cao (thi cử)", ipa: "/pɑːs wɪð ˈflaɪ.ɪŋ ˈkʌl.əz/", pos: "idiom", ex: "He passed the exam with flying colors." },
        { en: "Challenging but rewarding", vi: "Thử thách nhưng xứng đáng", ipa: "/ˈtʃæl.ɪn.dʒɪŋ bʌt rɪˈwɔː.dɪŋ/", pos: "adj. phrase", ex: "Teaching is challenging but rewarding." },
        { en: "Broaden my horizons", vi: "Mở rộng tầm mắt/kiến thức", ipa: "/ˈbrɔː.dən maɪ həˈraɪ.zənz/", pos: "v. phrase", ex: "Travel broadens my horizons." },
        { en: "Practical experience", vi: "Kinh nghiệm thực tế", ipa: "/ˈpræk.tɪ.kəl ɪkˈspɪə.ri.əns/", pos: "n. phrase", ex: "Internships provide practical experience." },
        { en: "Lucrative income", vi: "Thu nhập cao/hậu hĩnh", ipa: "/ˈluː.krə.tɪv ˈɪn.kʌm/", pos: "n. phrase", ex: "IT offers a lucrative income." },
        { en: "Make a living", vi: "Kiếm sống", ipa: "/meɪk ə ˈlɪv.ɪŋ/", pos: "v. phrase", ex: "It's hard to make a living as an artist." },
        { en: "Cover my bills", vi: "Trang trải chi phí sinh hoạt", ipa: "/ˈkʌv.ər maɪ bɪlz/", pos: "v. phrase", ex: "I need a job to cover my bills." },
        { en: "Promotion opportunities", vi: "Cơ hội thăng tiến", ipa: "/prəˈməʊ.ʃən ˌɒp.əˈtjuː.nə.tiz/", pos: "n. phrase", ex: "The company offers good promotion opportunities." },
        { en: "Get promoted", vi: "Được thăng chức", ipa: "/ɡet prəˈməʊ.tɪd/", pos: "v. phrase", ex: "She got promoted last month." },
        { en: "Soft skills", vi: "Kỹ năng mềm", ipa: "/sɒft skɪlz/", pos: "n. phrase", ex: "Soft skills are essential for teamwork." },
        { en: "Teamwork spirit", vi: "Tinh thần đồng đội", ipa: "/ˈtiːm.wɜːk ˈspɪr.ɪt/", pos: "n. phrase", ex: "We value teamwork spirit." },
        { en: "Job satisfaction", vi: "Sự hài lòng trong công việc", ipa: "/dʒɒb ˌsæt.ɪsˈfæk.ʃən/", pos: "n. phrase", ex: "Job satisfaction is important." },
        { en: "Stable job", vi: "Công việc ổn định", ipa: "/ˈsteɪ.bəl dʒɒb/", pos: "n. phrase", ex: "My parents want me to have a stable job." },
        { en: "Gap year", vi: "Năm nghỉ phép (trải nghiệm)", ipa: "/ɡæp jɪər/", pos: "n. phrase", ex: "I took a gap year to travel." },
        { en: "Located in / Situated in", vi: "Nằm ở...", ipa: "/ləʊˈkeɪ.tɪd ɪn/", pos: "adj. phrase", ex: "The hotel is situated in the center." },
        { en: "Coastal city", vi: "Thành phố biển", ipa: "/ˈkəʊ.stəl ˈsɪt.i/", pos: "n. phrase", ex: "Da Nang is a beautiful coastal city." },
        { en: "Mountainous area", vi: "Khu vực miền núi", ipa: "/ˈmaʊn.tɪ.nəs ˈeə.ri.ə/", pos: "n. phrase", ex: "They live in a mountainous area." },
        { en: "The suburbs / Outskirts", vi: "Vùng ngoại ô", ipa: "/ˈsʌb.ɜːbz/", pos: "n", ex: "We moved to the suburbs." },
        { en: "Heart of the city", vi: "Trung tâm thành phố", ipa: "/hɑːt əv ðə ˈsɪt.i/", pos: "n. phrase", ex: "My office is in the heart of the city." },
        { en: "Industrial zone", vi: "Khu công nghiệp", ipa: "/ɪnˈdʌs.tri.əl zəʊn/", pos: "n. phrase", ex: "The factory is in an industrial zone." },
        { en: "Tourist attraction", vi: "Điểm thu hút du lịch", ipa: "/ˈtʊə.rɪst əˈtræk.ʃən/", pos: "n. phrase", ex: "This museum is a major tourist attraction." },
        { en: "Picturesque landscapes", vi: "Phong cảnh đẹp như tranh", ipa: "/ˌpɪk.tʃərˈesk ˈlænd.skeɪps/", pos: "n. phrase", ex: "The region is known for picturesque landscapes." },
        { en: "Breathtaking view", vi: "Cảnh đẹp nín thở", ipa: "/ˈbreθˌteɪ.kɪŋ vjuː/", pos: "n. phrase", ex: "The room has a breathtaking view." },
        { en: "Historical sites", vi: "Di tích lịch sử", ipa: "/hɪˈstɒr.ɪ.kəl saɪts/", pos: "n. phrase", ex: "We visited many historical sites." },
        { en: "Pace of life", vi: "Nhịp sống", ipa: "/peɪs əv laɪf/", pos: "n. phrase", ex: "I enjoy the slow pace of life here." },
        { en: "Hustle and bustle", vi: "Sự hối hả nhộn nhịp", ipa: "/ˈhʌs.əl ənd ˈbʌs.əl/", pos: "idiom", ex: "I escaped the hustle and bustle of the city." },
        { en: "Tranquil / Peaceful", vi: "Yên bình", ipa: "/ˈtræŋ.kwɪl/", pos: "adj", ex: "The village is very tranquil." },
        { en: "Fresh air", vi: "Không khí trong lành", ipa: "/freʃ eər/", pos: "n. phrase", ex: "I love the fresh air in the morning." },
        { en: "Polluted", vi: "Ô nhiễm", ipa: "/pəˈluː.tɪd/", pos: "adj", ex: "The river is heavily polluted." },
        { en: "Traffic congestion", vi: "Tắc đường", ipa: "/ˈtræf.ɪk kənˈdʒes.tʃən/", pos: "n. phrase", ex: "Traffic congestion is bad during rush hour." },
        { en: "Commute", vi: "Việc đi lại (đi làm)", ipa: "/kəˈmjuːt/", pos: "n/v", ex: "My daily commute takes an hour." },
        { en: "Crowded / Packed", vi: "Đông đúc", ipa: "/ˈkraʊ.dɪd/", pos: "adj", ex: "The bus was crowded." },
        { en: "Vibrant", vi: "Sôi động, đầy sức sống", ipa: "/ˈvaɪ.brənt/", pos: "adj", ex: "The city has a vibrant nightlife." },
        { en: "Dull / Boring", vi: "Nhàm chán", ipa: "/dʌl/", pos: "adj", ex: "Life here can be dull." },
        
        // PART 2 (51-100)
        { en: "Hospitable", vi: "Hiếu khách", ipa: "/hɒsˈpɪt.ə.bəl/", pos: "adj", ex: "The locals are very hospitable." },
        { en: "Friendly and welcoming", vi: "Thân thiện và chào đón", ipa: "/ˈfrend.li ənd ˈwel.kəm.ɪŋ/", pos: "adj. phrase", ex: "The staff were friendly and welcoming." },
        { en: "Sense of community", vi: "Tinh thần cộng đồng", ipa: "/sens əv kəˈmjuː.nə.ti/", pos: "n. phrase", ex: "There is a strong sense of community." },
        { en: "Local delicacies", vi: "Đặc sản địa phương", ipa: "/ˈləʊ.kəl ˈdel.ɪ.kə.siz/", pos: "n. phrase", ex: "Try the local delicacies." },
        { en: "Street food", vi: "Đồ ăn đường phố", ipa: "/striːt fuːd/", pos: "n. phrase", ex: "Street food here is delicious." },
        { en: "Amenities", vi: "Các tiện ích", ipa: "/əˈmiː.nə.tiz/", pos: "n", ex: "The hotel has excellent amenities." },
        { en: "Entertainment center", vi: "Khu vui chơi giải trí", ipa: "/en.təˈteɪn.mənt ˈsen.tər/", pos: "n. phrase", ex: "Kids love the entertainment center." },
        { en: "Public transport system", vi: "Hệ thống giao thông công cộng", ipa: "/ˈpʌb.lɪk ˈtræn.spɔːt ˈsɪs.təm/", pos: "n. phrase", ex: "The public transport system is efficient." },
        { en: "Shopping mall", vi: "Trung tâm thương mại", ipa: "/ˈʃɒp.ɪŋ mɔːl/", pos: "n. phrase", ex: "We went to the shopping mall." },
        { en: "Undergo dramatic changes", vi: "Trải qua thay đổi mạnh mẽ", ipa: "/ˌʌn.dəˈɡəʊ drəˈmæt.ɪk ˈtʃeɪn.dʒɪz/", pos: "v. phrase", ex: "The city underwent dramatic changes." },
        { en: "Apartment block / Flat", vi: "Chung cư / Căn hộ", ipa: "/əˈpɑːt.mənt blɒk/", pos: "n. phrase", ex: "I live in a modern apartment block." },
        { en: "Terraced house", vi: "Nhà phố (nhà liền kề)", ipa: "/ˈter.əst haʊs/", pos: "n. phrase", ex: "We bought a terraced house." },
        { en: "Detached house", vi: "Nhà riêng biệt lập", ipa: "/dɪˈtætʃt haʊs/", pos: "n. phrase", ex: "A detached house offers privacy." },
        { en: "Dormitory", vi: "Ký túc xá", ipa: "/ˈdɔː.mɪ.tər.i/", pos: "n", ex: "Students live in the dormitory." },
        { en: "Rented accommodation", vi: "Nhà thuê", ipa: "/ˈren.tɪd əˌkɒm.əˈdeɪ.ʃən/", pos: "n. phrase", ex: "Rent accommodation is expensive." },
        { en: "Residential area", vi: "Khu dân cư", ipa: "/ˌrez.ɪˈden.ʃəl ˈeə.ri.ə/", pos: "n. phrase", ex: "It is a quiet residential area." },
        { en: "Convenient location", vi: "Vị trí thuận tiện", ipa: "/kənˈviː.ni.ənt ləʊˈkeɪ.ʃən/", pos: "n. phrase", ex: "The hotel has a convenient location." },
        { en: "Within walking distance of", vi: "Gần (có thể đi bộ tới...)", ipa: "/wɪˈðɪn ˈwɔː.kɪŋ ˈdɪs.təns əv/", pos: "phrase", ex: "The beach is within walking distance." },
        { en: "Prime location", vi: "Vị trí đắc địa", ipa: "/praɪm ləʊˈkeɪ.ʃən/", pos: "n. phrase", ex: "The shop is in a prime location." },
        { en: "Overlook (a park/lake)", vi: "(Cửa sổ/Ban công) nhìn ra...", ipa: "/ˌəʊ.vəˈlʊk/", pos: "v", ex: "The window overlooks the park." },
        { en: "Spacious", vi: "Rộng rãi", ipa: "/ˈspeɪ.ʃəs/", pos: "adj", ex: "The room is very spacious." },
        { en: "Cramped", vi: "Chật chội", ipa: "/kræmpt/", pos: "adj", ex: "The small room felt cramped." },
        { en: "Cozy", vi: "Ấm cúng", ipa: "/ˈkəʊ.zi/", pos: "adj", ex: "It's a small but cozy apartment." },
        { en: "Airy", vi: "Thoáng khí", ipa: "/ˈeə.ri/", pos: "adj", ex: "Big windows make it airy." },
        { en: "Stuffy", vi: "Bí bách", ipa: "/ˈstʌf.i/", pos: "adj", ex: "Open a window; it's stuffy here." },
        { en: "Fully furnished", vi: "Đầy đủ nội thất", ipa: "/ˈfʊl.i ˈfɜː.nɪʃt/", pos: "adj. phrase", ex: "We rented a fully furnished flat." },
        { en: "Modern appliances", vi: "Thiết bị hiện đại", ipa: "/ˈmɒd.ən əˈplaɪ.əns.ɪz/", pos: "n. phrase", ex: "The kitchen has modern appliances." },
        { en: "Decorate", vi: "Trang trí", ipa: "/ˈdek.ə.reɪt/", pos: "v", ex: "We decorated the room for the party." },
        { en: "Renovate", vi: "Sửa sang, nâng cấp nhà", ipa: "/ˈren.ə.veɪt/", pos: "v", ex: "They plan to renovate the old house." },
        { en: "Balcony", vi: "Ban công", ipa: "/ˈbæl.kə.ni/", pos: "n", ex: "I have plants on the balcony." },
        { en: "House chores", vi: "Việc nhà", ipa: "/haʊs tʃɔːrz/", pos: "n. phrase", ex: "We share the house chores." },
        { en: "Do the laundry", vi: "Giặt đồ", ipa: "/duː ðə ˈlɔːn.dri/", pos: "v. phrase", ex: "I do the laundry on Sundays." },
        { en: "Tidy up", vi: "Dọn dẹp", ipa: "/ˈtaɪ.di ʌp/", pos: "phrasal v.", ex: "Please tidy up your room." },
        { en: "Family gathering", vi: "Tụ họp gia đình", ipa: "/ˈfæm.əl.i ˈɡæð.ər.ɪŋ/", pos: "n. phrase", ex: "We have a family gathering every holiday." },
        { en: "Privacy", vi: "Sự riêng tư", ipa: "/ˈprɪv.ə.si/", pos: "n", ex: "I need some privacy." },
        { en: "Unwind / Chill out", vi: "Thư giãn", ipa: "/ʌnˈwaɪnd/", pos: "phrasal v.", ex: "Listening to music helps me unwind." },
        { en: "Housewarming party", vi: "Tiệc tân gia", ipa: "/ˈhaʊsˌwɔː.mɪŋ ˈpɑː.ti/", pos: "n. phrase", ex: "They threw a housewarming party." },
        { en: "Get on well with neighbors", vi: "Hòa thuận với hàng xóm", ipa: "/ɡet ɒn wel wɪð ˈneɪ.bərz/", pos: "v. phrase", ex: "We get on well with our neighbors." },
        { en: "Noisy neighbors", vi: "Hàng xóm ồn ào", ipa: "/ˈnɔɪ.zi ˈneɪ.bərz/", pos: "n. phrase", ex: "Noisy neighbors can be annoying." },
        { en: "Feel at home", vi: "Cảm thấy thoải mái như ở nhà", ipa: "/fiːl ət həʊm/", pos: "idiom", ex: "Please sit down and feel at home." },
        { en: "Actually / To be honest", vi: "Thật ra thì...", ipa: "/ˈæk.tʃu.ə.li/", pos: "adv", ex: "Actually, I don't like coffee." },
        { en: "Generally speaking", vi: "Nói chung là", ipa: "/ˈdʒen.ər.əl.i ˈspiː.kɪŋ/", pos: "phrase", ex: "Generally speaking, it's a good movie." },
        { en: "What I like most about X is", vi: "Điều tôi thích nhất ở X là...", ipa: "/wɒt aɪ laɪk məʊst.../", pos: "phrase", ex: "What I like most about this city is the food." },
        { en: "I’m really keen on", vi: "Tôi rất thích...", ipa: "/aɪm ˈrɪə.li kiːn ɒn/", pos: "phrase", ex: "I'm really keen on photography." },
        { en: "It allows me to", vi: "Nó cho phép tôi làm gì...", ipa: "/ɪt əˈlaʊz miː tu/", pos: "phrase", ex: "It allows me to express myself." },
        { en: "Once in a blue moon", vi: "Hiếm khi", ipa: "/wʌns ɪn ə bluː muːn/", pos: "idiom", ex: "I go there once in a blue moon." },
        { en: "Day in, day out", vi: "Ngày qua ngày", ipa: "/deɪ ɪn deɪ aʊt/", pos: "idiom", ex: "He works day in, day out." },
        { en: "For the most part", vi: "Phần lớn là", ipa: "/fɔːr ðə məʊst pɑːt/", pos: "phrase", ex: "For the most part, I agree." },
        { en: "On top of that", vi: "Thêm vào đó", ipa: "/ɒn tɒp əv ðæt/", pos: "phrase", ex: "On top of that, it's free." },
        { en: "Last but not least", vi: "Cuối cùng nhưng không kém phần quan trọng", ipa: "/lɑːst bʌt nɒt liːst/", pos: "phrase", ex: "Last but not least, thank you for coming." },

        // PART 3 (101-120)
        { en: "On a daily basis", vi: "Hàng ngày", ipa: "/ɒn ə ˈdeɪ.li ˈbeɪ.sɪs/", pos: "adv phrase", ex: "I exercise on a daily basis." },
        { en: "From time to time", vi: "Thỉnh thoảng", ipa: "/frɒm taɪm tu taɪm/", pos: "adv phrase", ex: "I visit the park from time to time." },
        { en: "Every now and then", vi: "Thỉnh thoảng", ipa: "/ˈev.ri naʊ ənd ðen/", pos: "adv phrase", ex: "We meet up every now and then." },
        { en: "Frequently", vi: "Thường xuyên", ipa: "/ˈfriː.kwənt.li/", pos: "adv", ex: "She frequently visits the library." },
        { en: "Hardly ever / Rarely", vi: "Hiếm khi", ipa: "/ˈhɑːd.li ˈev.ər/", pos: "adv", ex: "I hardly ever watch TV." },
        { en: "Make a habit of", vi: "Tạo thói quen làm gì", ipa: "/meɪk ə ˈhæb.ɪt əv/", pos: "v phrase", ex: "Make a habit of reading daily." },
        { en: "Get into the habit of", vi: "Bắt đầu thói quen gì", ipa: "/ɡet ˈɪn.tu ðə ˈhæb.ɪt əv/", pos: "v phrase", ex: "I got into the habit of jogging." },
        { en: "Kick the bad habit", vi: "Từ bỏ thói quen xấu", ipa: "/kɪk ðə bæd ˈhæb.ɪt/", pos: "v phrase", ex: "He wants to kick the bad habit of smoking." },
        { en: "Stick to a routine", vi: "Tuân thủ lịch trình/thói quen", ipa: "/stɪk tu ə ruːˈtiːn/", pos: "v phrase", ex: "Sticking to a routine helps productivity." },
        { en: "Tend to", vi: "Có xu hướng", ipa: "/tend tu/", pos: "v phrase", ex: "I tend to wake up early." },
        { en: "Without fail", vi: "Không bao giờ bỏ sót (đều đặn)", ipa: "/wɪˈðaʊt feɪl/", pos: "idiom", ex: "She arrives at 8 AM without fail." },
        { en: "Early bird / Morning person", vi: "Người hay dậy sớm", ipa: "/ˈɜː.li bɜːd/", pos: "n phrase", ex: "I am an early bird." },
        { en: "Wake up at the crack of dawn", vi: "Dậy khi tờ mờ sáng", ipa: "/weɪk ʌp æt ðə kræk əv dɔːn/", pos: "idiom", ex: "He wakes up at the crack of dawn to farm." },
        { en: "Hit the snooze button", vi: "Bấm nút hoãn báo thức", ipa: "/hɪt ðə snuːz ˈbʌt.ən/", pos: "v phrase", ex: "I always hit the snooze button." },
        { en: "Oversleep", vi: "Ngủ quên", ipa: "/ˌəʊ.vəˈsliːp/", pos: "v", ex: "Don't oversleep on exam day." },
        { en: "Have a nutritious breakfast", vi: "Ăn bữa sáng dinh dưỡng", ipa: "/hæv ə njuːˈtrɪʃ.əs ˈbrek.fəst/", pos: "v phrase", ex: "Have a nutritious breakfast for energy." },
        { en: "Skip breakfast", vi: "Bỏ bữa sáng", ipa: "/skɪp ˈbrek.fəst/", pos: "v phrase", ex: "Never skip breakfast." },
        { en: "Grab a quick bite", vi: "Ăn vội cái gì đó", ipa: "/ɡræb ə kwɪk baɪt/", pos: "v phrase", ex: "Let's grab a quick bite before we go." },
        { en: "Get ready for school", vi: "Chuẩn bị đi học", ipa: "/ɡet ˈred.i fɔː skuːl/", pos: "v phrase", ex: "I get ready for school at 7 AM." },
        { en: "Rush out the door", vi: "Lao ra khỏi nhà", ipa: "/rʌʃ aʊt ðə dɔːr/", pos: "v phrase", ex: "He rushed out the door to catch the bus." }
    ];

    // Tạo mảng riêng cho từng phần để dễ quản lý (logic hiển thị sẽ lọc từ allVocabulary)
    // Nhưng để đơn giản cho logic render, ta sẽ dùng slice từ allVocabulary
    let currentDeckIndex = 0; // 0: 1-50, 1: 51-100, 2: 101-120
    const decks = [
        { start: 0, end: 20, name: "Phần 1: Từ 1 - 20" },
        { start: 20, end: 40, name: "Phần 2: Từ 21 - 40" },
        { start: 40, end: 60, name: "Phần 3: Từ 41 - 60" },
        { start: 60, end: 80, name: "Phần 4: Từ 61 - 80" },
        { start: 80, end: 100, name: "Phần 5: Từ 81 - 100" },
        { start: 100, end: 120, name: "Phần 6: Từ 101 - 120" }
    ];

    // Init current list based on deck 0
    let currentList = allVocabulary.slice(decks[0].start, decks[0].end).map(item => ({...item, status: 'new'}));
    // Note: status needs to be persisted or reset on deck change? 
    // Simple version: Reset status when changing deck (or keep separate state objects if complex)
    // To keep it simple in this single file, we will re-generate the status map when switching decks, 
    // effectively resetting progress for that session on deck switch.

    let isReviewMode = false;
    let currentIndex = 0;
    let isRevealed = false;
    let availableVoices = [];
    let selectedVoiceIndex = -1;
    let readingRate = 0.7;

    const elements = {
        vnText: document.getElementById('vn-text'),
        enText: document.getElementById('en-text'),
        ipaText: document.getElementById('ipa-text'),
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
        speedDisplay: document.getElementById('speed-display'),
        btnReview: document.getElementById('btn-review'),
        deckSelect: document.getElementById('deck-select')
    };

    // --- DECK LOGIC ---
    function changeDeck() {
        currentDeckIndex = parseInt(elements.deckSelect.value);
        const range = decks[currentDeckIndex];
        
        // Reset state for new deck
        currentList = allVocabulary.slice(range.start, range.end).map(item => ({...item, status: 'new'}));
        currentIndex = 0;
        isReviewMode = false;
        elements.btnReview.classList.remove('active');
        
        loadCard(0);
        elements.statusMsg.innerText = `Đã chuyển sang ${range.name}`;
        setTimeout(() => elements.statusMsg.innerText = "", 2000);
    }

    // --- AUDIO ---
    function loadVoices() {
        availableVoices = window.speechSynthesis.getVoices();
        elements.voiceSelect.innerHTML = '';
        const defaultOption = document.createElement('option');
        defaultOption.value = -1;
        defaultOption.text = "Tự động chọn (Tốt nhất)";
        elements.voiceSelect.appendChild(defaultOption);
        availableVoices.forEach((voice, index) => {
            if(voice.lang.includes('en')) {
                const option = document.createElement('option');
                option.value = index;
                option.text = `${voice.name} (${voice.lang})`;
                if (index === selectedVoiceIndex) option.selected = true;
                elements.voiceSelect.appendChild(option);
            }
        });
    }
    
    if (speechSynthesis.onvoiceschanged !== undefined) {
        speechSynthesis.onvoiceschanged = loadVoices;
    }
    setTimeout(loadVoices, 100);

    function playAudio(text) {
        window.speechSynthesis.cancel();
        const utterance = new SpeechSynthesisUtterance(text);
        
        if (selectedVoiceIndex !== -1 && availableVoices[selectedVoiceIndex]) {
            utterance.voice = availableVoices[selectedVoiceIndex];
        } else {
            let preferredVoice = availableVoices.find(voice => 
                (voice.name.includes('Google') && voice.lang.includes('en')) || 
                (voice.name.includes('Premium') && voice.lang.includes('en')) ||
                (voice.name.includes('Samantha') && voice.lang.includes('en'))
            );
            if (!preferredVoice) preferredVoice = availableVoices.find(voice => voice.lang === 'en-GB' || voice.lang === 'en_GB');
            if (!preferredVoice) preferredVoice = availableVoices.find(voice => voice.lang.includes('en'));
            if (preferredVoice) utterance.voice = preferredVoice;
        }
        
        utterance.rate = readingRate; 
        utterance.pitch = 1.0;
        utterance.volume = 1.0;
        utterance.onerror = (e) => console.log('Speech error:', e);
        window.speechSynthesis.speak(utterance);
    }

    function toggleSettings() {
        const isHidden = elements.settingsModal.style.display === 'none' || elements.settingsModal.style.display === '';
        if (isHidden) { elements.settingsModal.style.display = 'flex'; if(availableVoices.length === 0) loadVoices(); } else { elements.settingsModal.style.display = 'none'; }
    }

    function updateVoiceSettings() { selectedVoiceIndex = parseInt(elements.voiceSelect.value); }
    function updateSpeedSettings() { readingRate = parseFloat(elements.speedRange.value); elements.speedDisplay.innerText = readingRate; }
    function testVoice() { playAudio("Hello, this is a test for English voice."); }

    // --- MAIN LOGIC ---
    function toggleReviewMode() {
        if (isReviewMode) {
            // Revert to full deck
            const range = decks[currentDeckIndex];
            // We need to preserve statuses. 
            // In this simple implementation, currentList IS the state. 
            // So if we were filtering, we need to go back to the full 'currentList' but that was filtered.
            // Actually, best way is to keep 'currentList' as the Working List.
            // But when switching modes, we filter.
            // Let's reload the deck from the master source but we lose status.
            // BETTER: We filter the current list for display but keep the main list in memory.
            // For simplicity in this file: 
            // We will just alert if 0 items. 
            // If switching OFF review mode, we go back to showing all items in current deck range?
            // Since we modified 'currentList' in place in previous code, let's fix that.
            // We will reload the deck to get back all items, but we lose status.
            // FIX: We won't support complex state persistence in this simple file. 
            // Review mode will filter the CURRENT list. Exiting it will reset the deck.
            alert("Chế độ ôn tập sẽ lọc danh sách hiện tại. Để quay lại, hãy chọn lại Phần trong menu.");
            
            const learningWords = currentList.filter(item => item.status === 'learning');
            if (learningWords.length === 0) {
                alert("Bạn chưa có từ nào 'Chưa thuộc' trong phần này!");
                return;
            }
            currentList = learningWords;
            isReviewMode = true;
            currentIndex = 0;
            loadCard(0);
            elements.statusMsg.innerText = "📝 Đang ôn tập từ chưa thuộc";
            elements.btnReview.classList.add('active');
        } else {
             // Already entered, maybe button acts as toggle off?
             // Since we overwrote currentList, we can't easily toggle back without losing status unless we stored it.
             // We will reload the deck.
             changeDeck(); // Reloads full deck
        }
    }

    function shuffleVocabulary() {
        for (let i = currentList.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1));
            [currentList[i], currentList[j]] = [currentList[j], currentList[i]];
        }
        currentIndex = 0;
        loadCard(0);
        elements.statusMsg.innerText = "🔀 Đã đảo thứ tự!";
        setTimeout(() => elements.statusMsg.innerText = "", 2000);
    }

    function loadCard(index) {
        if (currentList.length === 0) return;

        if (index < 0) currentIndex = currentList.length - 1;
        else if (index >= currentList.length) currentIndex = 0;
        else currentIndex = index;

        const item = currentList[currentIndex];
        
        // Show Vietnamese + POS
        elements.vnText.innerHTML = `${item.vi}<div class="pos-tag">${item.pos}</div>`;
        
        elements.enText.innerText = item.en;
        elements.ipaText.innerText = item.ipa;
        elements.exText.innerText = `Ví dụ: "${item.ex}"`;
        
        elements.answerArea.style.display = 'none';
        elements.reviewActions.style.display = 'none';
        elements.btnReveal.style.display = 'block';
        elements.btnReveal.disabled = false;
        elements.btnReveal.innerText = "XEM ĐÁP ÁN";
        elements.statusMsg.innerText = "";
        
        elements.progress.innerText = `CÂU ${currentIndex + 1} / ${currentList.length}`;
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
        playAudio(currentList[currentIndex].en);
        elements.btnReveal.style.display = 'none'; 
        elements.reviewActions.style.display = 'flex'; 
    }

    function playCurrentAudio() { playAudio(currentList[currentIndex].en); }

    function markStatus(status) {
        currentList[currentIndex].status = status;
        updateStatusBadge(status);
        setTimeout(() => { changeCard(1); }, 300);
    }

    function changeCard(step) { loadCard(currentIndex + step); }

    // --- MODALS ---
    function toggleList() {
        const isHidden = elements.listModal.style.display === 'none' || elements.listModal.style.display === '';
        if (isHidden) { renderList(); elements.listModal.style.display = 'flex'; } else { elements.listModal.style.display = 'none'; }
    }

    function renderList() {
        elements.listContent.innerHTML = '';
        currentList.forEach((item, index) => {
            const div = document.createElement('div');
            div.className = `list-item ${index === currentIndex ? 'active' : ''}`;
            let statusIcon = '⚪';
            if (item.status === 'learned') statusIcon = '✅';
            if (item.status === 'learning') statusIcon = '🔸';
            div.innerHTML = `
                <div style="display:flex; align-items:center;">
                    <span style="margin-right:8px; font-size: 12px;">${statusIcon}</span>
                    <strong>${item.en}</strong>
                </div>
                <div style="font-size:12px; color:#666;">${index + 1}</div>
            `;
            div.onclick = () => { currentIndex = index; loadCard(currentIndex); toggleList(); };
            elements.listContent.appendChild(div);
        });
    }

    function toggleStats() {
        const isHidden = elements.statsModal.style.display === 'none' || elements.statsModal.style.display === '';
        if (isHidden) { renderStats(); elements.statsModal.style.display = 'flex'; } else { elements.statsModal.style.display = 'none'; }
    }

    function renderStats() {
        const learnedCount = currentList.filter(i => i.status === 'learned').length;
        const learningCount = currentList.filter(i => i.status === 'learning').length;
        const newCount = currentList.filter(i => i.status === 'new').length;
        
        elements.statLearned.innerText = learnedCount;
        elements.statLearning.innerText = learningCount;
        elements.statNew.innerText = newCount;
        
        let recommendItems = currentList.filter(i => i.status === 'learning');
        elements.recommendList.innerHTML = '';
        
        if (recommendItems.length === 0) {
             elements.recommendList.innerHTML = '<div style="color:green; padding:10px; text-align:center;">Tuyệt vời! Không có từ nào cần ôn gấp trong phần này.</div>';
        } else {
            recommendItems.forEach(item => {
                const div = document.createElement('div');
                div.className = 'recommend-item';
                div.innerHTML = `🔸 <strong>${item.en}</strong>`;
                // Find original index in current list to jump to
                const idx = currentList.indexOf(item);
                div.onclick = () => { currentIndex = idx; loadCard(currentIndex); toggleStats(); };
                elements.recommendList.appendChild(div);
            });
        }
    }

    // Init
    loadCard(0);
</script>

</body>
</html>
